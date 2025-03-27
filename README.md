# Data-analyst-Biprojit-Eportfolio

**Exploratory Data Analysis**

**Project Description**

This project analyses the dataset "Vancouver City Public Art" to gain insights into public art installations in Vancouver. The dataset contains information such as artist names, artwork titles, locations, and other descriptive attributes. This project uses AWS services to explore the distribution, trends, and patterns within the dataset, aiding in better cultural and historical documentation.

**Project Title**

Exploring Vancouver's Public Art Landscape

**Objective**

The objective of this Exploratory Data Analysis (EDA) is to gain a deeper understanding of the "Vancouver City Public Art" dataset by identifying key trends, missing values, and distributions of different attributes. This phase aims to:

• Analyze the distribution of public art installations over time and geographic regions.
• Identify patterns in art mediums, installation years, current status and artist contributions.
• Detect missing values, outliers, and inconsistencies that may affect further analysis.
• Use Amazon Athena for querying and summarizing dataset insights.

**Dataset**

The dataset used is "public_art_artists.csv," sourced from Vancouver's Open Data Portal. The dataset contains information about public art installations across the city, including:
	
 •      ArtistID – Unique identifier for each artist.
 
 •	Artist Name: Name of the artist(s) who created the art piece.
	
 •	Title: The name of the artwork.

 •      Type : The category of public art, such as Sculpture, Mural, or Digital Art 
	
 •	Year Installed: The year the artwork was installed.
	
 •	Program – The program or initiative under which the artwork was commissioned.

 •	Status: The current status of the artwork (e.g., Active, Removed).
	
 •	Location: The geographic placement of the art installation. The name of the public site where the artwork is installed (e.g., parks, streets, plazas).

 •      Artist Profile & Website – URLs linking to artist information and additional resources

**Methodology**

**Data Collection:** The dataset was extracted from the Vancouver Open Data platform.

**Data Ingestion:** The dataset was stored in an Amazon S3 bucket (publicart-raw-bipro).

**Data Profiling:** Data profiling was conducted to get an overview of the dataset and assess data quality. Using AWS Glue DataBrew, the following key aspects were examined:

• Column completeness – Checking for missing values across different attributes.

• Data types – Ensuring correct formats for numerical and categorical fields.

• Duplicate records – Identifying redundant entries that need to be removed.

• Statistical summaries – Generating min, max, mean, and distribution counts for numeric columns.

**Exploratory Data Analysis:** AWS Glue DataBrew and Amazon Athena were used to understand trends, missing values, and outliers.

**Data Cleaning:** To ensure accuracy in further analysis, data cleaning was performed using AWS Glue DataBrew:

• Missing Values Handling: Missing artist names were flagged for further investigation. Null values in installation years were replaced with the most frequent year in that particular region.

• Duplicate Removal: Identified duplicate records based on title, artist name, and location and removed them.
	
• Standardization: Text formatting was corrected (e.g., renaming artist heading names for uniformity).

**Visualization:** To gain meaningful insights, Amazon QuickSight was used to create visualizations for key dataset attributes. Various visualization techniques are used to investigate public art data efficiently.

**Interpretation & Insights:** Based on the above findings, the following insights were drawn:

• Public Art Growth Over Time: There was a significant increase in installations during the 1990s and early 2000s, followed by a slight decline post-2015. Future projects should investigate funding trends and policy changes that may have influenced these fluctuations.
	
• Geographic Concentration of Art Installations: The majority of public art is concentrated in Downtown Vancouver, suggesting city planners prioritized high-footfall areas for installations. Efforts can be made to promote public art in underrepresented neighborhoods to enhance accessibility.
	
• Material Trends in Public Art: The dominance of bronze and steel suggests a preference for durable materials in public installations. The limited use of modern materials like LED-based art indicates an area for potential innovation in future installations.

**Tools and Technologies**

AWS S3 – Storage for raw data

AWS Glue DataBrew – Data preprocessing and profiling

Amazon Athena – Querying and analyzing data

AWS QuickSight – Data visualization

**Deliverables**

Cleaned Dataset – Stored in Amazon S3 after removing inconsistencies.

Exploratory Data Summary – Key statistics and missing value reports.

Visual Reports – Graphical representations of public art trends.

Actionable Insights – Recommendations for data-driven decision-making.

**Descriptive Analysis of Vancouver City Public Art**

**Project Description**

This project involves a detailed descriptive analysis of the “Vancouver City Public Art” dataset to uncover patterns and summarize key characteristics of the public art installations. The focus is on understanding the most common artists, frequently used art types, distribution of installation years, and the geographical spread of public art across Vancouver. By leveraging AWS services, we ensure efficient data processing and visualization for meaningful insights.

**Project Title**

Analyzing the Characteristics of Vancouver’s Public Art

**Objective**

The objective of this Descriptive Data Analysis (DDA) is to summarize the dataset’s main attributes and provide insights into the characteristics of Vancouver’s public art collection. This phase focuses on:
• Identifying the most frequent artists, artwork types, and installation years.
• Summarizing the geographical distribution of public art across different city locations.
• Understanding the status of art installations, including active vs. removed works.
• Providing quantitative statistics to assist in future policy and funding decisions.


**Dataset**

**Methodology**

**Tools and Technologies**

**Deliverables**

**Data Wrangling for City of Vancouver City Public Art**

**Project Description**

Project Title

Objective

Background

Dataset

Methodology

Tools and Technologies

Deliverables

Timeline

Data Quality Control of Vancouver City Public Art

Project Description

Project Title

Objective

Background

Scope

Methodology

Deliverables

Timeline

Descriptive Analysis of Scholarly Activities for Faculties Policy at UCW

Project Description

Project Title

Objective

Dataset

Methodology

Tools and Technologies

Deliverables

Data Wrangling for Scholarly Activities for Faculties Policy at UCW

Project Description

Project Title

Objective

Background

Dataset

Methodology

Tools and Technologies

Deliverables

Timeline

Data Quality Control of Scholarly Activities for Faculties Policy at UCW

Policy at UCW

Project Description

Project Title

Objective

Background

Scope

Methodology

Deliverables

**Timeline**
