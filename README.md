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
	
 •      ArtistID: Unique identifier for each artist.
 
 •	Artist Name: Name of the artist(s) who created the art piece.
	
 •	Title: The name of the artwork.

 •      Type: The category of public art, such as Sculpture, Mural, or Digital Art 
	
 •	Year Installed: The year the artwork was installed.
	
 •	Program: The program or initiative under which the artwork was commissioned.

 •	Status: The current status of the artwork (e.g., Active, Removed).
	
 •	Location: The geographic placement of the art installation. The name of the public site where the artwork is installed (e.g., parks, streets, plazas).

 •      Artist Profile & Website: URLs linking to artist information and additional resources

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
	
• Geographic Concentration of Art Installations: The majority of public art is concentrated in Downtown Vancouver, suggesting city planners prioritized high-footfall areas for installations. Efforts can be made to promote public art in underrepresented neighbourhoods to enhance accessibility.
	
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

• Summarize the distribution of art types, locations, and installation years.

• Identify the most common artists and frequently commissioned artwork types.

• Summarizing the geographical distribution of public art across different city locations.

• Understanding the status of art installations, including active vs. removed works.

• Providing quantitative statistics to assist in future policy and funding decisions.

**Dataset**

Same as above

**Methodology**

**Data Collection and Preparation**

• The dataset was extracted from Vancouver’s Open Data Portal and stored in an Amazon S3 bucket (publicart-raw-bipro).

• AWS Glue DataBrew was used for data profiling, allowing an assessment of missing values, duplicate records, and incorrect data formats.

• Data Cleaning involved handling Missing Values, where missing installation years were replaced using the most frequent year per location. Next, duplicate entries with identical artist names, titles, and locations were flagged and eliminated. Finally, standardizing text formatting of Artist names and location names that were formatted consistently for analysis.

The cleaned dataset is stored in a transformation bucket (publicart-trf-bipro).

**Descriptive Statistics:** Using Amazon Athena, Glue DataBrew were executed to summarize dataset attributes.

• Most Common Artists: Identified top contributors based on the number of public artworks.

• Top Artwork Types: Counted occurrences of each art type (e.g., sculptures, murals).

• Installation Trends: Analyzed public art installations by decade.

• Geographic Distribution: Mapped artworks across high-density vs. low-density regions.

• Status Analysis: Compared active, removed, and relocated artworks.

**Data Visualization:** Visualizations were created using Amazon QuickSight to represent key dataset trends and illustrate installation trends over time, unique artist IDs, year installed, and number of installations.

**Insights and Findings:** Based on the descriptive analysis, the following insights were drawn:

• Public Art Growth Over Time

• A few artists have contributed significantly to public art, while most artists have only a single installation.

• A significant increase in installations was observed during the 1990s and early 2000s.

• A decline in new installations post-2015 suggests changes in funding or policy priorities.

• A sharp rise in public art projects during the 1990s and early 2000s, possibly due to government initiatives or increased funding for cultural programs.

• Sculptures and Murals dominate Vancouver’s public art landscape, indicating a preference for physical and visual storytelling.

• Modern art forms such as digital/LED-based works are underrepresented, showing a gap in technological integration.

• Downtown Vancouver has the highest concentration of public art installations.

• Suburban and low-income areas have fewer artworks, indicating a potential cultural disparity.

• Around 75% of artworks remain active, while 25% have been removed or relocated, raising concerns about long-term maintenance and conservation.


**Recommendations:** Based on the analysis, the following recommendations are proposed:

• Promote Art in Underserved Areas: Public art projects should be extended to less-represented neighborhoods to ensure cultural inclusivity.

• Support Emerging Artists: Since a few artists dominate public art, initiatives should be implemented to encourage newer artists to participate.

• Monitor Funding Trends: Further research into budget allocations can help understand the decline in installations post-2015.

• Improve Artwork Preservation and Documentation: Implement better tracking mechanisms for relocated and removed artworks. Increase maintenance efforts for older installations to prevent unnecessary removals.

**Tools and Technologies**

Same as above

**Deliverables**

• Descriptive Statistical Report – Summarizing dataset characteristics.

• Cleaned Dataset – Processed and stored in AWS S3 for further analysis.

• Visual Reports – Graphical insights into public art trends.

• Actionable Recommendations – Data-driven suggestions for city planners and policymakers.

**Data Wrangling for City of Vancouver City Public Art**

**Project Description**

The goal of this project is to ensure the accuracy, consistency, and usability of Vancouver’s public art dataset by performing data wrangling. The dataset, sourced from the Vancouver Open Data Portal, contains information about public art installations, including artist names, artwork titles, locations, installation years, and mediums.
This project utilizes AWS services such as Amazon S3, Glue DataBrew, and Athena to clean, transform, and enhance the dataset, making it suitable for exploratory and predictive analysis. The key challenges involve handling missing values, standardizing formats, identifying duplicates, and enriching the dataset with additional attributes such as artist contributions and medium trends.

**Project Title**

Data Wrangling for Vancouver City's Public Art Landscape

**Objective**

The objective of this project is to perform end-to-end data wrangling on Vancouver’s public art dataset to ensure:

• Data accuracy – eliminating inconsistencies and errors.

• Data completeness – addressing missing values effectively.

• Data standardization – ensuring a uniform structure for all attributes.

• Data usability – enabling meaningful insights into Vancouver’s public art scene.

By applying structured data processing techniques, this project enhances the dataset’s reliability for further analysis in cultural research, public art planning, and historical documentation.

**Background**

Vancouver is home to a rich and diverse collection of public art installations, spanning sculptures, murals, and digital artworks. The dataset provides a comprehensive view of these installations, but several data quality issues hinder effective analysis.

• Missing values in attributes like Year Installed, Artist Name, and type.
• Duplicate entries for certain artworks and artists.
• Inconsistent text formatting, such as capitalization differences in artist names.
• Incomplete location details, affecting geographical analysis.

Addressing these challenges through data wrangling is crucial for ensuring a reliable dataset that supports meaningful insights into public art distribution and trends.

**Dataset**

Same as above

**Methodology**

**1. Data Collection**

The dataset was extracted from the Vancouver Open Data Portal and uploaded to an Amazon S3 bucket (publicart-raw-bipro) for centralized and secure storage.

✔️ Data Security: AWS KMS encryption and S3 bucket versioning were enabled to maintain data integrity.

✔️ Access Control: IAM policies restricted unauthorized access to the dataset.

✔️ Data Backup: Raw datasets were preserved before transformation.

**2. Data Assessment**

Using AWS Glue DataBrew, an initial assessment of the dataset was performed to identify quality issues:

✔️ Missing Values: Artist Name (4%), Year Installed (7%), and type (5%) contained null values.

✔️ Duplicate Records: 3% of the dataset had duplicate records for artworks.

✔️ Inconsistent Formatting: Variations in capitalization and abbreviations in Artist Name and Location.

✔️ Statistical Summaries:

• The earliest recorded installation was 1950, while the most recent was 2023.

• The most common medium was Bronze, followed by Steel and Concrete.

**3. Data Cleaning**

Handling Missing Values

✔️ Missing Artist Names were flagged for manual review.

✔️ Missing Year Installed values were replaced with the mode year for that location.

✔️ Missing artwork name values were assigned based on similar artworks by the same artist.

Duplicate Removal

✔️ Duplicates were identified based on a combination of Title, Artist Name, and Location and removed using AWS Glue transformations.

Standardizing Data Formats

✔️ Converted Year Installed to integer format.

✔️ Standardized text fields to ensure consistent casing (e.g., Joe David instead of john david).

✔️ Normalized Medium values (e.g., merging bronze and Bronze into Bronze).


**Tools and Technologies**

**Deliverables**

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
