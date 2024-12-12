import datetime
import os

def organize_files_by_date(folder_path):
    """
    Organizes files in the specified folder into subfolders by their creation date.
    """
    if not os.path.exists(folder_path):
        print(f"Folder '{folder_path}' does not exist!")
        return

    for file_name in os.listdir(folder_path):
        file_path = os.path.join(folder_path, file_name)

        if os.path.isfile(file_path):
            creation_time = os.path.getctime(file_path)
            date_folder = datetime.datetime.fromtimestamp(creation_time).strftime('%Y-%m-%d')
            date_folder_path = os.path.join(folder_path, date_folder)

            if not os.path.exists(date_folder_path):
                os.makedirs(date_folder_path)

            os.rename(file_path, os.path.join(date_folder_path, file_name))
            print(f"Moved '{file_name}' to folder '{date_folder}'")

if __name__ == "__main__":
    folder_to_organize = input("Enter the folder path to organize: ")
    organize_files_by_date(folder_to_organize)
