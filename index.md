# Electronic Traineeship Notebook (ETN)

## Table of Contents
1. [Traineeship Documentation Plan](#TDP)   
    1.1. [Tentative Planning](#TDP1)    
    1.2. [Data Management](#TDP2)   
    1.3. [Traceability of Steps and Methods](#TDP3)  
    1.4. [Version Control of Code](#TDP4)   
2. [Background information traineeship topic](#background)  
3. [Reflection and self-directed behaviour](#refl)  
    3.1 [Personal Development](#pers-dev)   
    3.2 [Formative evaluation](#from-ev)	
    3.3 [Critical Reflection](#crit-refl)	
4. [Tasks](#tasks)  
    4.1. [✔️ Exploration of raw data formats from HPLC instrument](#task1)   
    4.2. [✔️ Download and install DELPHI repository](#task2)     
    4.3. [❌Create a "visitor" for raw HPLC data and generate tsv file](#task3)   
    4.4. [❌ Deal with compressed data HPLC files](#task4)   
    4.5. [✔️ Exploration raw UPLC data](#task5)   
    4.6. [✔️ Align on need for UPLC data upload format](#task6)   
    4.7. [❌ Meta-Analysis UPLC data](#task7)    
    4.8. [✔️ Upload Ion Chromatography data](#task8)     
    4.9. [✔️ Generate PDFs from UPLC data](#task9)       
    4.10. [✔️ Add inhouse IC data to pdf generation](#task10)       
    4.11. [✔️ Establish IC data as new cannical type on DELPHI](#task11)         
    4.12. [✔️Membrane Assay Preprocessing and analysis](#task12)        
    4.13. [✔️ Batch mass /volume calculator app](#task13)       
    4.14. [✔️Net Peptide Content Upload](#task14)

# Traineeship Documentation Plan <a name="TDP"></a>

## Tentative Planning <a name="TDP1"></a>
- Look into DELPHI the Disqover data platform that serves as AelinTx's one stop shop for data on research & development activities. -> Continuous
- Upload external Ion Chromatography data -> finished 26/02
- Build further robustness and pre-analysis IC data -> Finished 21/03
- HPLC vistor script -> Stopped
- Upload of UPLC data -> Finished 21/03
- Find a way to decompress .lcra files. -> Stopped
- Increase robustness PDF generation -> Finished 24/03
- Appending IC data to PDF generation -> Finished 07/04
- Establish IC data as new cannonical type -> Finished 12/04
- Membrane Assay Analysis -> Finished 31/05
- Batch mass / volume calculator app -> Finished 29/04
- Net Peptide Content Upload -> Finished 07/06


## Data Management <a name="TDP2"></a>
Data about the progress of the traineeship project will be stored according to the FAIR principles in this ETN.

**Findable**

Different tasks are listed at the start of the ETN and linked to their respective headers within the ETN.  

**Accessible**

The ETN is publicly available and a link is shared with the project coordinators. The repository of the code is stored in a private git repository that requires authentication and only the project coordinators will be allowed access as some of the data stored is not meant to be publicized.

**Interoperable**

Where possible a link to code written for the traineeship is supplied at the start of the task.

**Reusable**

The code repository is private, as the data used is confidential in nature. Descriptions in the ETN do not include any confidential data such as Pept-In:tm: codes or sequences, or any other identifiers that could allude to this data and it is therefore licensed under MIT.

## Traceability of Steps and Methods <a name="TDP3"></a>
This git repository markdown page will be used to document the project steps and changes in the project in a traceable manner.

## Version Control of Code <a name="TDP4"></a>

The code will be stored in [this private git repository](https://github.com/TVR-AelinTX/traineeship). 
Access will be given to the internal and external traineeship coordinators before the start of the traineeship. 
Links to scripts pertaining to tasks and subtasks of the traineeship will be provided in the ETN and can be accessed by the authorized coordinators.

# Background Information traineeship topic <a name="background"></a>

## HPLC
For the purification of the peptides manufactured in the lab, a method on a Reverse Phase High Performance Liquid Chromatography (RP-HPLC) system is used. The reverse phase points to the fact that a hydrophobic stationary phase is used, while the mobile phase initially is more hydrophilic in nature. The peptide is dissolved and injected with a constant flow of mobile phase into a column, the stationary phase. After several minutes the gradient of the mobile phase is shifted towards a more hydrophobic end. The peptide and its impurities bound to the column then each have their own 'sweet spot' of hydrophobicity where they will start prefering the mobile phase over the column and they will elute. This principle is used to separate the peptide of interest from any unwanted side-products from synthesis.

## UPLC
To analyze the purity of the peptides, an Ultra High Performance Liquid Chromatography (UPLC) system is used. It's concepts and inner workings are essentially the same as that of the HPLC, save for the higher pressure used in this system and the denser column material. This makes for a more efficient separation of analytes, but a higher retention time. This makes the system ideal for analytical purpose, while the HPLC is used for preparative purposes.

## Ion Chromatography
Another main source of variability between different peptide batches are the ion contents. Three ion types are analyzed in the lab (TFA, acetate and chloride) as these three are routinely used as counterions for the peptides. The software and principle are similar to the UPLC, except that the column now binds and separates ions with the use of positively charged beads that slow elution of the negative ions. 


## DELPHI
The DELPHI platform is AelinTx's source for data and information related to ongoing research and development activities. It is a tool build upon the [DISQOVER](https://www.ontoforce.com/platform/disqover/) semantic search platform that enables researchers and managers to quickly find the data they need from the ELN stored. DELPHI's main strength is its flexibility to adapt to any data source, trough the use of python coding, without disrupting the data flow. Additionally some routines can be written to expedite data analysis.

# Reflection and self-directed behaviour <a name="refl"></a>

## Personal Development <a name="pers-dev"></a>
**Concept of learning outcome**

Over the course of the traineeship, I will gain the skills and experience needed to familiarize myself with the DELPHI ELN-platform to help it grow by adding pre-processing, data uploading and curating subroutines to the pipeline. This will support my colleagues with their data management and allow for more reproducible experiments.

**Development activities**

- Python scripting: pandas, file IO
- Teamwork and communication: meetings with stakeholders, git
- Data visualization: R and Python, dashboards in DELPHI

**Desired results**

- Automatically generate a pdf summarizing some of the QC results of the lab in a clean and orderly manner.
- Process .txt, .xml files to extract the relevant information and upload it in a structured, curated manner
- Clearly communicate expectations, possibilities and changes related to projects to stakeholders and work together to achieve the best solution.

**Schedule**

The different activities run in parallel as they're heavily intertwined and give feedback to one another.

**Nescessary support and facilities**

Feedback is given when needed or whenever I feel stuck with a certain problem by the external coordinator. The course units of BIT provide support in handling issues (eg: Databases & Data Management, Python Scripting, Data Visualization).

**Conclusion**

The script to automatically generate PDFs was completed and incorporated existing quality data and newly uplaoded IC and UPLC data. Discussions are in progress to even further expand this script to include more data, that still needs to be generated or uploaded to DELPHI. Furthermore a tool was written to utilize quality data and structural data of the compounds and batches to allow calculation of a more precise concentration of analyte. 

## Formative Evaluation <a name="form-dev"></a>

**Feedback during traineeship**

- Testing, testing, testing: Test the code more often and early. Ideally after every piece of code that is added which changes something. 
- Expect the unexpected: When validating data from user input, try to be prepared for any format or type of typo's/errors and try to find ways to enforce data validation during data entry and some post-entry data cleanup routines.
- Communicate with the stakeholders: I've kept the stakehoders in the loop of the status of the project, so that any ideas or changes to the format could be implemented early on and there were no surprises in delivery of the project un terms of content or timeline.

**Intermediate Evaluation Form**

The evaluation was as expected, getting to know DELPHI went smooth and I could work on the different projects quite independently.
In the second part of the traineeship I would like to ramp up the difficulty and combine python programming with some JavaScript for making some front end changes on the DELPHI user interface. 

## Critical Reflection <a name="crit-refl"></a>

**Self-assesment**

- LO1:
    - Applies relevant programming techniques to process (biological) information in an automated manner: 
	Excellent. In the code written, many different python libraries are used. Some of which were known to me, others I had got to know during the traineeship. 
    - Programmes as efficient as possible: 
	Good. I try to tackle problems in the most efficient way possible, but need more experience and could time functions or test out different aproaches to make sure it is the most efficient method.
- LO2:
    - Efficiently and critically adjusts the structure of a self-developed or existing program: 
	Good. I can improve previous code upon reflection and with some testing, as I've done many times during the traineeship.  
    - Efficiently and critically adjusts the structure and the content of a given (biological) data file: 
	Excellent. Many files had to be read, stored into pandas DataFrames and preprocessed during the traineeship.
- LO3:
    - Autonomously selects and deposits biological data from or in a database, whether or not in an automated manner: 
	Excellent. This was the premise of most projects for the traineeship. Scrape through raw data files and retrieve relevant data for DELPHI to store it and display it. 
    - Develops new database structures to manage existing or acquired biological data: 
	NA. A json file was generated and updated with timestamps of data acquisition, but this is hardly a database system. 
    - Develops a (web) interface to process (biological complex) data in a user-friendly and efficient manner: 
	Excellent. Setting up the views on DELPHI, developing a calculator app embedded into the page, using plotly to add some dynamic elements to plots.
- LO4:
    - Takes initiative to actively search and use new application possibilities in the field of bioinformatics: 
	Excellent. I have looked for new python libraries and ways of processing and visualizing data during this traineeship.
    - Expands his current knowledge of data structures and programming skills and autonomously adjusts contributing to a
more efficient retrieval and processing of data for a given biological problem: 
	Good. Not every library I have come across resulted in a contribution to the projects.
    - Takes into account the legislation, regulations, (international) standards and values, and applies them in order to
protect the data privacy: 
	Good. At Aelin our Peptins(tm) are our greatest asset and therefore there is always an air of confidentiality around the company. Data processed only lives on the internal server here at the company. 
- LO5:
    - Critically evaluates the possibilities to analyse the given or acquired, whether or not in an automated manner,
(biological) data: 
	Good. I have tried out and compared different methods for the projects at times, but would need more experience in applying different methods to form my own insights. I did sometimes consult my colleagues on their opinions.
    - Autonomously selects the appropriate software to process the given or acquired, whether or not in an automated
manner, (biological) data: 
	Good. I have written some code in javascript for the calculator tool, to allow for dynamic interactions with the user. I have also written some bash scripts to help with the data flow.
- LO6:
    - Combines multiple disciplines, but herby strictly holds to his own domain: 
	Excellent. During the process of writing scripts to preprocess the data I have consulted the scientists working with the data for validation of my methods of analyzing and interpreting the raw data and gathering their feedback. 
    - Analyses, synthesizes and harmonizes inferences from different disciplines up to a coherent and coordinated level: 
	Excellent. The conclusion of (almost) each project is a pandas Dataframe containing all the elements calculated or extracted for a certain id of a sample/batch.
- LO7:
    - Reports results and information according to the standards valid in the work field: 
	Excellent. I try to add plenty of comments to my code and use the commit messages in a clear and succinct way.
    - Shows a participatory attitude towards the organisation and the team: 
	Excellent. I prefer to share my work with colleagues and ask for their insights as there is always something to learn that way. I am also always happy to lend a hand where needed.

**Reflection on international/intercultural aspects**

Aelin is a company with many international colleagues. Official communication is always done in English: mail, Teams, documentation. 
Inofficial communication is done in Dutch and French. There are only two sites at the present, both in Belgium: Ghent and Heverlee. 

# Tasks <a name="tasks"></a>
## Exploration of raw data formats from HPLC instrument <a name="task1"></a>
### 01/02/2022: 
First look at the data with exploratory [jupyter notebook](https://github.com/TVR-AelinTX/traineeship/blob/main/data_exploration/HPLC/HPLC%20Data.ipynb)

### 08/02/2022: 
Fixing further issues with the parsing of the .lcra files. Script should be simplified, but entanglement of different samples in one file and no clear way to link them makes this difficult...
### 10/02/2022: 
Extracting raw data using pandas.read_xml to get a clearer dataframe to start with. 
A setting in the package needs to be adapted however to allow handling files of this size.

## Download and install Delphi repository <a name="task2"></a>
### 01/02/2022: 
Download repo and installing dependencies.

Install, explore and use Pycharm. Issues using WSL interpreter (only supported in professional version). 
Continued using VS Code for now, perhaps come back to pyCharm later.

### 08/02/2022:
Facing issues testing out the visitor script using VSCode. Tried switching to PyCharm again, using WSL graphic interface. Ran into issues due to not being able to contact graphic server (firewall issues?). 
### 10/02/2022:
Sat together with external coordinator and fixed the issue. 

## Create a "visitor" that checks for new HPLC experiments on the server. <a name="task3"></a>

Link to copy of script that has been encapsulated in the DELPHI structure: [hplc_visitor.py](https://github.com/TVR-AelinTX/traineeship/blob/main/hplc/hplc_visitor.py)

### 03/02/2022:
Mock directory containing some raw files that aren't compressed made to target with a visitor script. 

"Visitors" are a python object that looks at folders and retrieves new, updated files according to some specifications. A visitor for the HPLC data would need to be made that  tracks changes in raw .lcra files during DELPHI's data ingestion.

### 08/02/2022:
Incorporated methods distilled from the data exploration into the visitor script. Needs more work refining and restructuring. Issues testing code on local computer.

### 10/02/2022:
Fixed issues testing visitor script on local computer. Issue not clearly defined, but seems to be related to naming conventions of folders (to keep in mind!). 

Script was appended with new methods and debugged to a workable state. More finetuning needed by adding a lookup file before execution of the script. The script now generates plots for all the peptides in a .lcra file. It uses a standard gradient (can be improved by selecting the right gradient) for now as most often the HPLC runs use the same gradient and identifying the gradient with the run proves not to be straightforward, as gradients of preparatory and finishing gradients are also recorded. The plots look good on most runs, altough some seem to be missing fractions (to be investigated). The plots could also be prettified further.

### 22/02/2022:
Using pandas to read the data from the xml-like files is memory intensive and requires changing some lines of code in the pandas library. Therefore a re-write of the code to use a personalized handler that only extracts the needed data from the xml file in one go is initiated.

### 24/02/2022:
Finalizing the reader. Started linking the data to the Chromatogram class, which needs a rework to fit with the new structure.

### 01/03/2022: 
Work on the HPLC data was shelved in favor for looking at the UPLC data.

## Deal with compressed .lcra raw HPLC files. <a name="task4"></a>
### 03/02/2022:
Some .lcra files exported from the machine undergo a compression to reduce the impact of their size on the system. 

Finding a way to read these compressed files is needed to visualize the chromatograms contained in them. No immediate settings were found to prevent this behaviour on the machine, so the company was contacted.

Some settings in the data acquisition could help generate reports with the needed data. This should first be investigated, alternatively the data is compressed on sql level and the company providing the sql database could be contacted by the supplier of the instrument for further help.

### 08/02/2022:
Asked to contact the company providing the sql database interaction from the software.

### 24/02/2022:
Response from the supplier. There is a special module for sale that could extract the data in a non encrypted format. Discussion for the need of this investment is needed.

### 01/03/2022:
It was decided not to purchase the module after further discussion. The work on the HPLC data was put on hold, as the fraction of uncompressed data is minimal compared to that of the compressed data. 

## Exploration raw UPLC Data. <a name="task5"></a>
### 08/02/2022:
Handling the UPLC raw data is much more straightforward. It can be exported in two .txt files per QC run performed. One file contains raw measurements to recreate the chromatogram, the other the area under the curve (AUC) per retention time calculated by the software of the UPLC.

### 15/02/2022:
UPLC data was explored. The software can spit out .txt files of the raw data and integration results. Parsing of both files and retrieving the interesting data with python is quite effective.

## Align on need for UPLC data upload format. <a name="task6"></a>
### 10/02/2022:
The possibility of uploading the UPLC data was discussed and the QC representative showed an interest, but wanted to first set in place more methods (Ion Chromatography) to analyze the peptides, which could be added to the reporting.

### 15/02/2022:
The need for upload of externally acquired Ion Chromatography data was adressed in a meeting. After sitting together with the external project coordinator, it was decided to work on this first. This is achieved by utilizing upload schemes of the DELPHI platform (xlsx files defining fields of pandas dataframes, templates, etc) and some internal logic.

### 10/03/2022:
A script was written to automate the transfer of UPLC exported data on the lab instruments in a specified folder to the server. During transfer a "_uplc" tag is provided to the text files as metadata to distinguish the files from raw ic data in the future. 

## Meta Analysis UPLC data. <a name="task7"></a>
### 15/02/2022:
For two different methods the absorbance is measured at wavelengths 210nm and 216nm respectively. It would be easy to unionize this reading by only looking at one of both wavelengths. Therefore an analysis of previous UPLC runs needs to be made to show that the resulting purity(%) values between the two different wavelength measurements does not differ significantly.

A bash script was written to pick up and put together the files from a list of exported files. A python script is written that extracts retention time, sample name and detector wavelength. Next step is to compare both groups statistically.

### 17/02/2022:
A first exploratory visual analysis of the data reveals some differences between both readings for some samples. The distribution of the differences was tested for normalcy and the null hypothesis that the distribution was normal was rejected at a significance of 0.05.

### 22/02/2022:
A second set of same sample readings was analyzed. Here the differences between both reading are normally distributed. A student t-test confirms that the difference between both datasets of the same sample is significant. Purities calculated by both methods for different samples show no significant difference accoring to a Wilcoxon's signed rank test.  

### 01/03/2022:
The measurements at 210 nm are selected as the absorbance there is of a greater intensity. Further analysis is put on hold.  

## Upload Ion Chromatography data to DELPHI platform <a name="task8"></a>

Link to copy of script that has been encapsulated in the DELPHI structure: [import_dlph_compounds_batches](https://github.com/TVR-AelinTX/traineeship/blob/main/ion_chrom/import_dlph_compounds_batches.py)

### 15/02/2022:
A basic scheme for uploading data on the resulting ion percentages from ion chromatography experiments is made to allow upload onto the DELPHI platform. Upload schemes consist of excel sheets defining input and output fields for the data that is read from an excel template. These schemes are used by the internal logic of DELPHI in the form of python script to pre-process, ingest and display the data on the web platform.

Some basic logic is added to the script to preprocess the data.

### 17/02/2022:
The scheme is updated with fields for the date of upload, the person uploading the data and the location of the data to ensure traceability.

The internal logics are also polished with some data validation and cleanup to allow a more robust pre-processing. Ideas for future improvements: classification by main ion, comparison of salt_state vs experimental_salt_state.

### 22/02/2022:
Testing the code on the production server led to errors involving the merging of the IC data to the batch data. The code was rewritten in a more memory efficient way and the joining of the dataframes was adapted to not produce any errors.

### 24/02/2022:
The code was tested on the production server and yielded no errors. The change was communicated to the rest of the team and data upload was initiated.

### 10/03/2022:
The presentation of the results was embellished trough the use of html and css and a python script that dynamically allocates colors based on fractions of values. 

### 15/03/2022:
The formatting was further optimized and the three divs whee joined in a container div with flexbox properties to account for different viewports. Replacing three fields to the data ingestion dataframe by one field of the combined results.


## Generate PDFs UPLC data <a name="task9"></a>
### 01/03/2022:
An automated method to generate certificates of analysis from the data obtained by UPLC would be a useful implementation for the company. 

The backbones for the script are tested out and written in [this jupyter notebook](https://github.com/TVR-AelinTX/traineeship/blob/main/data_exploration/UPLC/UPLC%20DATA%20exploration.ipynb). The means to extract the raw data from .txt files are written and a first small pdf was generated.

### 03/03/2022:
A [more thorough pdf generation backbone script](https://github.com/TVR-AelinTX/traineeship/blob/main/uplc/pdf_report.py) was made using reportlab. It takes variables from the delphi tables to supplement the raw data with other compound and batch related properties.

### 07/03/2022:
Incorporation of pieces of the code into DELPHI started. The process is as follows: a [visitor script](https://github.com/TVR-AelinTX/traineeship/blob/main/uplc/delphi_scripts/uplc_qc.py) will scrape the ELN for new raw UPLC data (posted in a monthly folder) and retrieve relevant data needed for the report. It will also generate a chromatogram and save it to the server to be displayed on DELPHI and included in the report.

After this, an [operation script](https://github.com/TVR-AelinTX/traineeship/blob/main/uplc/delphi_scripts/gen_batch_qc_reports.py) will join tables from batches, compounds and the uplc data to get all the relevant data for the report. This data is then fed to a function that generates the report. The function is wrapped by a method that keeps track of any changes and only runs the code when there are changes. 

### 10/03/2022:
The pdf generation was further polished and formatting was adapted to ammeliorate more extreme input data (eg. large integration tables).

### 15/03/2022:
The method for finding the UPLC data was improved to allow for nested directories. An error showed up and was traced to differences in regionality between used computers (lab vs DELPHI server). A date was printed in "%d.%b.%Y" format in German on the lab instrument, which was not recognized by the script on the server. The script was appended with the dateparser library to translate this format.

### 17/03/2022:
A button was styled in html and css to allow viewing the pdf from the batches dashboard. The code was tested on the sandbox server and a few bugs were fixed after testing. 

### 21/03/2022:
Some of the images urls did not allow for viewing the UPLC chromatograms. This was due to a '#' in the filename which causes the url not to function properly. The '#'s were replaced by 'n's in the script before url generation to allow the chromatograms to be displayed. The way of merging the UPLC data with the batch data in pandas was also adapted to prevent duplication of batches.

### 24/03/2022:
The code was wrapped in some error handling to report different parts of the code where things could go awry.

## Add inhouse IC data to pdf generation <a name="task10"></a>

### 21/03/2022:
The Ion Chromatography data was explored initially in [a jupyter notebook](https://github.com/TVR-AelinTX/traineeship/tree/main/data_exploration/IC). The program used to process and export the IC data, Chromeleon, is the same as for the UPLC. This way a similar workflow could be set up to get the data exported to the server and read in by Delphi.

Some settings needed to be changed on the Chromeleon software to allow a one-click export by the user. Structure of the saved runs was also copied to that of the UPLC data, for inner consistency.

### 24/03/2022:
A bash script was written to transfer the data exported to the backport in the server to a permanent place in the server. During transfer an '_ic' metatag is added to the filenames.

Further preprocessing of the IC data was worked on in the jupyter notebook.

### 29/03/2022:

The [script for handling the IC data](https://github.com/TVR-AelinTX/traineeship/blob/main/ion_chrom/ic_qc.py) was incorporated into DELPHI and tested on the sandbox.

### 07/04/2022:

Incorporation of the IC data into the generated PDFs. Formatting of the figures and pdf.

## Establish IC data as new canonical type on DELPHI <a name="task11"></a>

### 29/03/2022:

It was decided to make the IC data their own category of data on DELPHI, to accomodate comparison of different measurements (on different dates, different technical replicates or from different sources). The masterdata was set up to create this new cannonical type and an [operation](https://github.com/TVR-AelinTX/traineeship/blob/main/ion_chrom/import_dlph_ic_data.py) was written to preprocess and add the IC data to it.

### 31/03/2022:

The code was refactored further and the data was linked to batches and vice versa. Changes were tested on sandbox and further polishing of the code was done.

### 05/04/2022:

The dashboard on the sandbox server was adapted to properly display the IC data in its new cannonical type (front end).  

### 12/04/2022:

The IC data standard curves were polished and a typo in the parameters of the script was corrected. The PDF layout was uniformized to have a more cohesive look and feel. A workflow was written for uploading the IC raw data to the ELN.

## Membrane Assay Preprocessing and analysis <a name="task12"></a>

### 14/04/2022:

It was proposed to have a look at membrane disruption data for the second half of the internship as the pdf generation project was comming to an end. The experiments are done in 96 well plates. Data needed for these experiments comes from two sources that should be linked to eachother: the raw data with the absorbance readings of the experiment and then some sort of template to be designed that indicates what sample corresponds to which well. Some data exploration was done in [this notebook](https://github.com/TVR-AelinTX/traineeship/blob/main/data_exploration/membrane_leakage/membrane_assay.ipynb).

### 19/04/2022:

The initial thought was to design a template that looks like a well plate to easily assign a sample per well and keep an overview of the plate. Due to the many different conditions possible between wells during an experiment (concentration, sample, buffer, membrane type, ...) an alternative aproach was chose to define well per well these variables. Some logic was thought out to allow designing ranges of dilution series, to allow for more efficient data entry. Regular expression was used to make a list of well numbers or letters from a string using following syntax:

A:E -> [A,B,C,D,E]
A&E -> [A,E]

Combining these with dilution series of the same length, a pandas explode forms a dataframe of the ranges that can be used to define samples well per well.

### 21/04/2022:

Plots were generated of the test data. Data was grouped per compound, concentration and batch and then the means of the replicates was used for plotting. A script was written that plots per compound the different concentrations in another color and displays the sample with the max absorbance (lysed membrane) and a negative control (membrane without disruption).

### 26/04/2022:

The averages of the measurements were smoothed using [scipy.signal.medfilt](https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.medfilt.html). The results of these filter are compared to the original using a find_peaks call. If the resulting amount of peaks is the same or only 1 less peak is found the peak is labeled as a 'bad peak' with too much signal noise and it is displayed in gray and pushed to the back of the plotting layer.

A strategy was searched for to try and mitigate these 'bad peaks' by removing noisy measurements from the averaging done in pandas, but no strategy was found yet.

### 29/04/2022:

Refactoring of the code to the operations level of DELPHI to allow a more centralized processing of plate reader experiments. Multiple plate reader formats are used by different instruments and this would allow cross-compatibility of parsing different formats for different experiments.

### 03/05/2022:

Filtering out the noisy, 'bad' peaks by calculating the standard deviation on the 80th and 90th percentile absorbance measurements. The curves plateau at the end of the assay in the case of a stable measurement, but at the end of the assay the liposomes are lysed and the signal then further increases to the maximum absorbance value. Therefore it is important to compare these plateaus before the lysis between differen measurements for anomalous noise levels. The mean of the standard deviations of measurements at each concentration of the experiment are calculated and curves with a standard deviation that are at least 1.6 times higher than the mean are marked as 'bad curves', greyed out on the plots and not used in further calculations for the EC50.

### 05/05/2022:

Further refactoring of the preprocessing script for a more readable and organized structure. 
One plot per sample is generated instead of a summary plot of all the samples.

### 10/05/2022:

Improvements to the plate template syntax for expanding well ranges were made to handle more edge case scenario's.
 
### 12/05/2022:

The area under the curve for the absorbance curves is calculated and normalized versus the triton (maximum signal) and vehicle (background signal) sample areas under the curve.
An EC50 plot is generated with this normalized AUC versus the log concentration. Historically a five parameter logistic regression was fitted to these curves [using the GraphPad program](https://www.graphpad.com/guides/prism/latest/curve-fitting/reg_asymmetric_dose_response_ec.htm). 
This logistic regression fit was coded in python using scipy.optimize's curve_fit function with the formula `d + ((a-d) / np.power((1 + np.power((x/c), b)), e))`   

### 17/05/2022:

The plate reader part of the script was refactored to the visitor level, using a new data structure to uniformize the processing of plate assay data further. Mathias had written the visitor as an variant of the standard template visitor used in DELPHI. 
The visitor was modified with rules on how to deduce which type of plate is used and how to process the raw data file by scraping the metadata.

### 19/05/2022:

The code was further refactored and prepared for a first test in the sandbox environment. Inconsistencies were found during testing between output on the sandbox and local testing. After some searching the plate syntax part of the code seemed to be the culprit as it was using the pandas.explode function on multiple columns. This feature was released in pandas v1.3, while the pandas version running on production and sandbox was pandas 1.1.3.

### 24/05/2022:

An upgrade of pandas was performed on the sandbox environment to test if this would solve the issue, but it broke other pieces of the DELPHI code. Therefore it was decided to momentarily cut the plate syntax functionality from the platereader for the time being and reset to pandas v1.1.3.
The rest of the code ran fine under the old pandas version and the templates for displaying the output on DELHI were configured.

### 31/05/2022:

The summary plots were made dynamically using plotly. Poorly behaving curves (significantly higher standard deviation than the average) were plotted as dashed lines (to indicate they are not used in further calculation) and then hidden by default.
The user can click the concentration of these plots to set them to visible, should they want a summary plot that does show these curves.
The final code can be found [here](https://github.com/TVR-AelinTX/traineeship/blob/main/membrane_assay/import_dlph_membrane_disruption.py)

The plate syntax functionality was wrapped in a tkinter dialog script and compiled to a .exe usable by the scientists with pyinstaller.


## Batch mass /volume calculator app <a name="task13"></a>

### 21/04/2022:

The idea was proposed to add a calculator to our batches of compound on the ELN that takes into account the molarity of the compound and (in the future) the net peptide compound of our batches to allow for correct weighing and dilluting of the compounds for experiments. The idea was to add a html div with some Javascript code and dynamically add information of the batches/compounds from the ELN through Python. 

### 26/04/2022:

A first draft of the calculator was [written a codepen](https://codepen.io/TheOafidian/pen/VwygRvj) that already includes the brunt of the JS, the html structure and styling done using [bootstrap](https://getbootstrap.com/) as not to waste too much time on styling.

### 29/04/2022:

Code injection could be kept to a minimum by inserting the calculator as an iframe with as source an html page including the js logic. The dynamic parameters can be supplied to the script using a query (eg: src="calculator.html?mw=2000&npc=0.75").  

#### Interactive example
<iframe src="https://htmlpreview.github.io/?https://github.com/TVR-AelinTX/calc_example/blob/main/calc.html?mw=2000&npc=0.75" scrolling='no' style="border: none;" height='400px' width="500px"></iframe>
[source code](https://github.com/TVR-AelinTX/traineeship/blob/main/batch_calculator/Calculator.html)

## Net Peptide Content Upload <a name="task14"></a>

### 27/05/2022:

Measurements of the net peptide content per batch are being performed recently. This data could be added to the batch calculator to take this peptide content into account per specific batch for molarity calculations.
The data needs to be uploaded to DELPHI for the batch calculator tool to use these values in the iframe. A simple upload tempalte was deviced that does some data validation and then prioritizes certain NPC methods of measuring above others (due to higher accuracy of the measurements method) to assign an NPC value to a batch based on which measurements are uploaded.
The priority of the methods was set up as follows KF > AAA > UPLC
A timestamp system is set up to keep track of the current and previous NPC values per batch. This way a previously calculated molarity can be recalculated if new, more accurate and deviating NPC values are obtained.

### 31/05/2022:

The calculator was tested to see if the npc data was added as a query to the html string in the correct batches.

### 07/06/2022:

NPC measurements can be done at two different moments. Before aliquotation of the batch by lyophilization and after this lyophilization. For calculation purposes the first can only be used if a whole vial of peptide (generally 4mgs is dissolved, while the latter is used if manual wheighing is performed to dissolve a known quantity of peptin.
The code was refactored to take into account this distinction and save two npc values per batch. 
Additional code was written to take into account KF measurements, where the water content is measured. Combining this water content with IC data from a batch the NPC should equal 100% deducted by the % of ions measured by IC and the water content % by Karl Fisher.
The final code can be found [here](https://github.com/TVR-AelinTX/traineeship/blob/main/npc_upload/import_dlph_npc_data.py)


[//]: # (Intermediate Evaluation Traineeship)

[//]: # (Self Assessment at the End of Traineeship)

[//]: # (Reflection on International/Intercultural Aspects)

<script src="https://unpkg.com/vanilla-back-to-top@7.2.1/dist/vanilla-back-to-top.min.js"></script>
<script>addBackToTop({
  diameter: 56,
  backgroundColor: 'rgb(0,128,128)',
  textColor: '#fff'
})</script>
