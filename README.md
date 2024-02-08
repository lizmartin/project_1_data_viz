# project_1_data_viz
Team Strong Minds | Project 1 Data Visualization
Contributors: Lisa Tschudi, Kelsy Dysart, Liz Martin-Strong

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

Summary:
We improved our skills on choosing our analysis questions, use of Github, coding with python pandas and matplotlib and describing our results.
We found no statistical correlation* between number of healthcare facilities and population, per capita income, nor median age in each zip code.
We found data combining and visualization relatively easy compared to formulating questions, locating appropriate data sets and version control.  We realized too late for presentation deadlines that our results are incorrect in that we have zip code counts(those on the outside of the city) which are artificially low.  We were originally going to reduce results from our facility search by radius to just those in the defined zip codes we wanted to include(drawing the circle a bit larger than Denver itself).  We forgot to drop the ones for which we have partial counts.

Ideas for future work:
*Refine our coding to get complete facility results from each zip code which we include(by dropping results from zip codes we do not choose to include from the geoapify results drawn by radius).  We currently have zip codes for which we have an artificially low healthcare facility count, which we realized too late to correct for this presentation.
 Investigate wheelchair access to facilities in Denver, CO healthcare facilities.  We were very curious about this due to two group members’ lived experiences.  We noticed a data point was included from geoapify for each facility about wheelchairs.
Explore the various healthcare categories on their own.  It would be interesting to see if there is any more noticeable correlation between facility count and our demographics if we only look at one category, or exclude some(for example, exclude pharmacies which often sell a lot more items than only medical prescriptions).
Widen the geographic area of this project, or perform similar analysis for other cities.  

Folders: 
**output_data**: conatins the three files pulling data from Geoapify PlacesAPI to gather healthcare facilities information for Denver zip codes
1. additional_facilities.csv
2. denver_healthcare_data.csv
3. first_500_facilites.csv

**resources**: contains csv data for of zipcodes and healtcare facilities created by making API calls. What the team used to generate visualizations.
1. combined_data.csv
2. denver_heathcare_data.csv
3. denver_zipcodes.csv

**visuals**: contains all outputs of our visualization coding.
1. Lisa completed question 1 and map visualizations:
    denver_map_categories.png
    denver_map_population.png
    pop_facilities_denver_plot.png
    pop_facilities_denver_scatter.png
2. Liz completed question 2
    income_hcf_by_denver_zip.png
    income_scatter.png
3. Kelsy completed question 3 
    med_age_and_facilities_multi_bar.png
    med_age_and_facilities_scatter.png

**wheelchair_questions**: contains Kelsy Dysart's preliminary work to explore wheelchair access on 
1. test_geo_healthcare.ipynb tests with limited set what results will look like
2. test_geo_healthcare_wheelchair.ipynb gives a sample of the results for limiting the condition to wheelchair access

**workings_files**: contains the workbooks created for parts of the larger project. Some work has been added into the "main_project1.ipynb" file
1.den_healthcare_1.ipynb - Kelsy's work. Used to make API call to GeoApify to generate output data
2. den_healthcare_2.ipynb - Kelsy's work. Used to make API call to GeoApify to generate output data
3. sample_geo_healthcare.ipynb
4. zipcode_by_city_name.ipynb

**Root level files**:
1. main_project1_final_doc - Everyone's work: Overall development plan. Lisa's work for building data frame and making API call for data from State of Colorado.  
2. question_1_vis_final.ipynb - Lisa's work for visualizations
3. question_2_vis.ipynb - Liz's work for visualizations
4. question_3_vis.ipynb - Kelsy's work for visualizations
5. Folder also includes the final presentation and summary of our work: UO_Data_Viz_Project_1.pptx

