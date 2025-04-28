# A2: Conda Environment
The goal of this assignment is to recreate two environments from the files located in this repository: https://github.com/augustinh22/geo-software-dev/tree/main/A2

- *software_dev_v1.yml*
- *software_dev_v2.yml*

## 1. Cloninng the Reporsitory and Copying Folder A2 to Personal Folder
The repository was cloned using the following command. Then, the A2 folder was copied and pasted into the local destination folder (PLUS_softwaredev_2025_NicoleSalazar).
```bash
git clone https://github.com/augustinh22/geo-software-dev.git 
cp /Users/nicolesalazar/geo-software-dev/A2 /Users/nicolesalazar/Documents/MASTER/CDE/S2/PSD/repos/PLUS_softwaredev_2025_NicoleSalazar
```

## 2. Pushing the New Folder to GitHub
Now, it is necessary to commit the local changes to the repository **PLUS_softwaredev_2025_NicoleSalazar** by running the following commands:
```bash
git add .
git commit -m "Copied A2 content from original repo"
git push origin main
```
<img width="982" alt="Screenshot 2025-04-28 at 1 06 59 PM" src="https://github.com/user-attachments/assets/1cf945dd-d9d5-471f-8d91-8f5c74477200" />

## 3. Replicating Environments
### 3.1 Environment 1 (software_dev_v1.yml)
#### 3.1.1 Creating the Environment V1
After running the command ```bashconda env create -f software_dev_v1.yml``` the following error was encountered:

<img width="981" alt="Screenshot 2025-04-28 at 3 18 59 PM" src="https://github.com/user-attachments/assets/92be5abb-0374-46e0-aa6a-8113d453bc23" />

The reason is that some packages have dependencies that are only supported on Windows, not on Mac. To fix this error, it was necessary to remove the conflicting dependencies and run the code snippet again.

<img width="983" alt="Screenshot 2025-04-28 at 3 24 44 PM" src="https://github.com/user-attachments/assets/6071cf68-eb00-4c3d-841b-c65d0e7dd3f1" />

#### 3.1.2 Activating the environment V1
No errors occured during this step.

<img width="545" alt="Screenshot 2025-04-28 at 3 31 52 PM" src="https://github.com/user-attachments/assets/84b005e1-bac5-427b-9828-86b6743ea90a" />

### 3.2 Environment 2 (software_dev_v2.yml)
#### 3.2.1 Creating the Environment V2
To create the second environment was necessary to desactivate the environment one by runing this command:

```bash
conda deactivate
```

The environament *software_dev_v2.yml* was succesfully created with not error.

<img width="979" alt="Screenshot 2025-04-28 at 4 20 09 PM" src="https://github.com/user-attachments/assets/14c584c3-018b-4ec7-be5c-226ef16fd575" />


#### 3.2.2 Activating the Environment V2
No errors found during this step.

<img width="743" alt="Screenshot 2025-04-28 at 4 25 49 PM" src="https://github.com/user-attachments/assets/f2577070-afa0-4f20-9e8c-86e8cd36590b" />

## 4. Verifying the Conda Environments
To verify that the environments were correctly set up, the command ```bash conda env list``` is used.

<img width="566" alt="Screenshot 2025-04-28 at 4 38 25 PM" src="https://github.com/user-attachments/assets/bf44dae6-73b3-4012-b241-a2970f07e276" />

The image above confirms that the environments were successfully set up and are operational.
