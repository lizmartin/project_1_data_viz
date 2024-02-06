# project_1_data_viz
Strong Minds | Project 1 Data Visualization
Formulating questions:
Lisa had an interest in the broad subject of family caregivers, particularly parents of children with intellectual disability and what contributes to their wellbeing. 
Data to answer questions around this was not easily publicly available.
Suspected it was an under researched question
Explored the Census data set
This has a complicated data schema and API call architecture. 
We had difficulty formulating a specific question with data we could use and switched to a healthcare ‘deserts’ idea, suggested by our teacher, investigating the concentration of healthcare facilities as we also have an interest in that. 

We wanted to know more about access to health care services. 
Our work was modeled loosely off the Banking Desert exercise from class. 
We were curious if health care services were concentrated in geographic regions due to:
Higher population numbers
Income level
Age
Selected a large metro area – Denver, Colorado


Folders: 


**resources**: contains csv data for of zipcodes and healtcare facilities
1. denver_heathcare_data.csv

**workings_files**: contains the workbooks created for parts of the larger project.
1. den_healthcare_1.ipynb
2. den_healthcare_2.ipynb
3. sample_geo_healthcare.ipynb
4. zipcode_by_city_name.ipynb

**wheelchair_questions**: contains Kelsey Dysart's preliminary work to explore wheelchair access on 
1. test_geo_healthcare.ipynb tests with limited set what results will look like
2. test_geo_healthcare_wheelchair.ipynb gives a sample of the results for limiting the condition to wheelchair access

**output_data**: conatins the three files pulling data from Geoapify PlacesAPI to gather healthcare facilities information for Denver zip codes
1. additional_facilities.csv
2. denver_healthcare_data.csv
3. first_500_facilites.csv 

Summary:
We improved our skills on choosing our analysis questions, use of Github, coding with python pandas and matplotlib and describing our results.
We found no statistical correlation* between number of healthcare facilities and population, per capita income, nor median age in each zip code.
We found data combining and visualization relatively easy compared to formulating questions, locating appropriate data sets and version control.  We realized too late for presentation deadlines that our results are incorrect in that we have zip code counts(those on the outside of the city) which are artificially low.  We were originally going to reduce results from our facility search by radius to just those in the defined zip codes we wanted to include(drawing the circle a bit larger than Denver itself).  We forgot to drop the ones for which we have partial counts.

Ideas for future work:
*Refine our coding to get complete facility results from each zip code which we include(by dropping results from zip codes we do not choose to include from the geoapify results drawn by radius).  We currently have zip codes for which we have an artificially low healthcare facility count, which we realized too late to correct for this presentation.
 Investigate wheelchair access to facilities in Denver, CO healthcare facilities.  We were very curious about this due to two group members’ lived experiences.  We noticed a data point was included from geoapify for each facility about wheelchairs.
Explore the various healthcare categories on their own.  It would be interesting to see if there is any more noticeable correlation between facility count and our demographics if we only look at one category, or exclude some(for example, exclude pharmacies which often sell a lot more items than only medical prescriptions).
Widen the geographic area of this project, or perform similar analysis for other cities.  

