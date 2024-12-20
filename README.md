# Higher Diploma in Computing - Data Analytics Module Assessment - Module: Computer Infrastructure
![photo of ATU Galway](https://www.midwestradio.ie/images/Image_of_ATU_Sligo_Campus.jpg)
This repository contains my work for the assessment components due on **Friday, 20 December 2024**.

## Purpose of the Assessment

The goal of this assessment is to demonstrate the following abilities:
- Use, configure, and script in a command line interface environment.
- Manipulate and move data and code using the command line.
- Compare commonly available software infrastructures and architectures.
- Select appropriate infrastructure for a given computational task.

## Repository Contents

This repository is structured to be clear, concise, and professional for technical review or potential use in interviews. Below is a breakdown of its contents:

### Directory Structure
```
├── data/
│   ├── timestamps/
│   ├── weather/
├── .github/
│   └── workflows/
├── weather.sh
├── weather.ipynb
├── weather-data.yml
├── .gitignore
├── README.md
```

### Key Files and Directories
- **`data/`**: Contains subdirectories for timestamp and weather data.
  - **`timestamps/`**: Stores timestamp files generated during tasks 2-4.
  - **`weather/`**: Stores weather data files downloaded from Met Éireann and data from tasks 5-7.
- **`weather.sh`**: Bash script automating weather data downloads and timestamping.
- **`weather.ipynb`**: Jupyter Notebook containing a report summarizing the tasks, Python analysis of weather data using pandas, and insights into the dataset.
- **`.github/workflows/weather-data.yml`**: GitHub Actions workflow for automating daily weather data downloads and repository updates.
- **`.gitignore`**: Specifies files and directories to exclude from version control.
- **`README.md`**: Provides an overview of the repository and its contents.

---

## Assessment Components

### Tasks (40%)
1. **Create Directory Structure**: Organized directories for storing data files.
2. **Timestamps**: Generated and formatted timestamps using command line tools.
3. **Create Timestamped Files**: Created timestamped files with formatted names.
4. **Download Weather Data**: Automated retrieval of Met Éireann weather data.
5. **Timestamp the Data**: Applied timestamped naming to downloaded files.
6. **Write the Script**: Developed `weather.sh` to automate the above processes.
7. **Notebook Report**: Documented tasks, commands, and their purpose in `weather.ipynb`.
8. **Analyse Weather Data**: Utilized `pandas` to analyse and summarise weather data.

### Project (40%)
- Created a GitHub Actions workflow (`weather-data.yml`) to:
  - Run `weather.sh` daily at 10 AM using a Linux virtual machine.
  - Automatically commit and push updates to the repository.

### Repository Management (20%)
- Maintained a consistent and professional commit history.
- Structured the repository for clarity and ease of use.
- Ensured code and documentation are well-organized and accessible.

---

## How to Use This Repository

### Prerequisites
#### Run locally
- Install [Visual Studio Code](https://code.visualstudio.com/Download) as it is an ideal shell to use locally.
- Install [Anaconda](https://www.anaconda.com/download/success) this will give you python with additional packages. 
- Install [Git](https://git-scm.com/) and clone this repository:
  ```bash
  git clone https://github.com/AndreHoarau/computer_infrastructure_assessment/tree/main
  ```
#### Run in the cloud
- Navigate to your github account.
- If you do not have a repository made yet make one [How to make a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories)
- Then navigate to *code* and select [*launch codespaces*](https://docs.github.com/en/codespaces/developing-in-a-codespace/creating-a-codespace-for-a-repository)

#### Regardless of local run or cloud
- Install the required Python packages:
  ```bash
  pip install -r requirements.txt
  ```

### Running the Script applicable to both local and cloud
- Make `weather.sh` executable:
  ```bash
  chmod +x weather.sh
  ```
- Run the script:
  ```bash
  ./weather.sh
  ```

### Viewing the Notebook
Open `weather.ipynb` in Jupyter Notebook to explore the task explanations and data analysis.
This can be done either in the visual studio code through the file explorer.
Alternatively on windows open cmd prompt
```
cd <location of cloned repository>
jupyter notebook
```


---

## GitHub Actions Workflow

The `weather-data.yml` workflow automates the daily execution of `weather.sh`:
- **Schedule**: Runs daily at 10 AM and can be triggered manually.
- **Steps**: 
  - Clone the repository.
  - Execute `weather.sh`.
  - Commit and push new weather data.

To review the workflow logs, navigate to the **Actions** tab in the GitHub repository.

---

## Feedback and Progress

Regular commits and structured updates reflect the progress throughout the semester. Feedback provided during lectures has been incorporated into the work.

---

## License

This project is licensed for educational purposes under ATU Galway's guidelines located on the [StudentHub](https://studenthub.atu.ie/).

---

## Acknowledgements

Thanks to [Dr. Ian McLoughlin](https://github.com/ianmcloughlin) for guidance throughout the semester, and to [Met Éireann](https://www.met.ie/climate/available-data) for providing the weather data used in this project.

---

For any questions or feedback, feel free to reach out to me on [LinkedIn](https://www.linkedin.com/in/andre-hoarau/)
