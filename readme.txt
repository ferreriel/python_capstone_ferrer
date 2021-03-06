Since volunteering with local organization Louisville Grows, I learned that Louisville is one of the lowest-ranked cities in the country for tree canopy density, loses canopy every year, and is consistently labeled as a heatsink. One of the arguments Louisville Grows states when they encourage residents to engage in their Urban Forestry program is that trees help reduce local temperature and save on energy bills. For this project I aimed to investigate if increased tree canopy had a measurable reduction in local temperature. 

Information on the data is provided by the [Louisville Urban Tree Canopy Assessment](https://louisvilleky.gov/sites/default/files/community_forestry/community_foresty_files/louisvilleutcreport-24march2015_draft.pdf). 
Average surface temperatures for each neighborhood are based on 5x5 meter grid measurements derived from surface temperature grid satellite imagery. Land surfaces are grouped into 3 categories in the data csv file: tree canopy, grass/low vegetation, and impervious surfaces combined with bare soil. Impervious surfaces and bare soil lumped together is simplified later to impervious surface, in that it does not mitigate water nor heat. Ultimately I chose to calculate a ratio of impervious ground to pervious ground by dividing the impervious & bare soil percent by the sum of tree canopy and vegetation percent.

Dependencies
Setup uses pandas, matplotlib, sqlite3, seaborn
Related to seaborn: upgrade to scipy 1.2 if you encounter "FutureWarning".
On [FutureWarning](https://stackoverflow.com/questions/52594235/futurewarning-using-a-non-tuple-sequence-for-multidimensional-indexing-is-depre) if scipy isn't version 1.2.
