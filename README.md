# RTPS Voter Management System

A web-based application for managing voter data organized by Subdivision, Block, Panchayat, and Polling Station. The application allows users to browse the hierarchical data and upload Excel files to update the data structure.

## Features

- Hierarchical dropdown navigation (Subdivision → Block → Panchayat)
- Display polling station data in a tabular format
- Upload and process Excel files to update the data structure
- Generate updated data.js file for easy deployment
- Responsive design that works on desktop and mobile devices

## How to Use

### Viewing Data

1. Select a Subdivision from the dropdown menu
2. Select a Block from the dropdown menu (enabled after selecting a Subdivision)
3. Select a Panchayat from the dropdown menu (enabled after selecting a Block)
4. Click the "Search" button to display polling stations for the selected Panchayat

### Uploading Data

1. Prepare an Excel file (.xlsx or .xls) with the following columns:
   - Subdivision
   - Block
   - Panchayat
   - PollingStationNo
   - PollingStationName
   - Location
   - TotalVoters
   - MaleVoters
   - FemaleVoters
   - OtherVoters

2. Click the "Browse" button in the Data Upload section
3. Select your Excel file
4. Click the "Upload and Update Data" button
5. The application will process the file and generate an updated data.js file
6. Download the updated data.js file and replace the existing one in your project

## Excel File Format

The Excel file should have a single sheet with the following columns:

| Subdivision | Block | Panchayat | PollingStationNo | PollingStationName | Location | TotalVoters | MaleVoters | FemaleVoters | OtherVoters |
|-------------|-------|-----------|------------------|---------------------|----------|-------------|------------|--------------|-------------|
| Sub1        | Blk1  | Pan1      | 1                | PS Name 1           | Loc1     | 1000        | 500        | 495          | 5           |
| Sub1        | Blk1  | Pan1      | 2                | PS Name 2           | Loc2     | 1200        | 600        | 595          | 5           |
| Sub1        | Blk1  | Pan2      | 3                | PS Name 3           | Loc3     | 900         | 450        | 445          | 5           |
| Sub1        | Blk2  | Pan3      | 4                | PS Name 4           | Loc4     | 800         | 400        | 395          | 5           |
| Sub2        | Blk3  | Pan4      | 5                | PS Name 5           | Loc5     | 1100        | 550        | 545          | 5           |

## Hosting on GitHub

### Setting Up a GitHub Repository

1. Create a GitHub account if you don't have one already
2. Create a new repository on GitHub
3. Initialize the repository with a README file

### Uploading the Application to GitHub

1. Clone the repository to your local machine
2. Copy all the application files to the cloned repository folder
3. Commit the changes and push to GitHub

```bash
git add .
git commit -m "Initial commit of RTPS Voter Management System"
git push origin main
```

### Enabling GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings"
3. Scroll down to the "GitHub Pages" section
4. Select the branch you want to deploy (usually "main")
5. Click "Save"
6. GitHub will provide you with a URL where your application is hosted

## Updating Data on GitHub

1. After uploading an Excel file and generating a new data.js file
2. Replace the existing data.js file in your local repository
3. Commit and push the changes to GitHub

```bash
git add data.js
git commit -m "Update voter data"
git push origin main
```

4. The changes will be automatically reflected on your GitHub Pages site

## Technical Details

- The application is built using HTML, CSS, and JavaScript
- Bootstrap 5 is used for responsive design
- SheetJS (xlsx) is used for Excel file processing
- No server-side code is required, making it easy to host on GitHub Pages

## License

This project is licensed under the MIT License - see the LICENSE file for details.