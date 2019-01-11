# Craigslist-Job-Listing-Transformation-via-Text-Modeling

Abstract :

Inspire Analytica consults Craigslist on ways to increase the traffic on their job portal. One of the main reasons identified is the lack of structure in job postings. Inspire Analytica, a group of students, suggest ways to improve the structure of these web sites using NLP and machine learning techniques that they acquired over the period of their course ‘Analyzing Unstructured Data’.

About Job Search Market :

As per the Bureau of Labor Statistics, more than 2 million Americans voluntarily leave their jobs every month and look for new opportunities. Combining these numbers with involuntary unemployment, means that there are a lot of people looking for jobs at any given point of time. The top channels people use to look for new jobs are online job boards (60%), social professional networks (56%), and word of mouth (50%). Global job portal revenue rose 9% in in 2016, reaching $12.4 billion with LinkedIn and Monster as the largest players in the US. Other job portals in the US include indeed.com, simplyhired.com. 

Problem Statement :

Craigslist also offers the facility of posting advertisements related to jobs on their portal, but this category is not nearly as popular as similar websites like monster.com or indeed.com. It has a lot of job listings that are classified into very broad categories. When a user navigates through the listings, he/she can only see the date on which the job was posted and the title. The title is a user’s free input text, thus, there is not format or structure. Recruiters use fancy words to attract traffic. But they lack the basic information about the position for which the job is posted. 
Additionally, users can’t find most of the relevant information such as employment type, compensation, the name of the organization unless he clicks on the link. This lack of information on the search page forces the user to click on the links only to find that the job is not suitable for him, which could be for any number of reasons. Given a large number of job postings, it is humanely impossible to navigate through 100s of pages. Thus, even when there are 1000s of jobs available, because of the lack of text architecture, the purpose of matching a recruiter’s need to user’s remains difficult.

Proposal : 

Improve the quality and presentation of the job listings on Craigslist website to enhance the user experience, drive more traffic to the website and thus increase the revenue. 
We are proposing to change the way these posts are listed on Craigslist so that job-seekers have an easy time navigating the portal and can easily find the relevant jobs. We believe that this will lead to an enhanced user experience, which will drive more traffic to the website and encourage job-providers to list on the website. Considering that job-listings are charged by Craigslist, it will increase the revenue of the client. 

Solution :

We used the SVM model to predict the titles for jobs listed on Craigslist using the job descriptions. We had a total of 120 data points under ‘Business and Management’ category. Since, the job titles were not available to cross-validate, we manually created these labels based on job description. 
Using these manually labelled titles as original data, we calculated the accuracy using predicted values from SVM model. 
In the model, we observed that we were able to predict the Job Title accurately for 42 cases out of 120. This puts our accuracy for Craigslist at 35%. These are followed by those jobs who were tagged partially. There were 34 such cases, which accounted for 28% of the jobs. 
To better understand this behavior, we must first remember that the model works on Key-word tagging. Once, tokenized, sentences no longer retain contextual meaning. This makes it difficult for NLP algorithms to predict all entities in a sentence. In our case, we had 1000 job listings from Indeed and over 300 titles to which these jobs belonged. 
Due to a lack of data, the model is not able to identify all keywords associated with various job titles. This is reflected in its behavior while partially tagging reviews.
The performance of the model can be improved by training it on more data. Currently, more than a third of the data consists of unique labels. For building an accurate model we will need more data points with fewer classification labels.

Conclusion  :

We believe that implementing the model will be very helpful to the Craigslist. It will have an impact on employers as well as the job-seekers. Since the jobseekers will have an easy time navigating the platform and extracting the relevant information without even clicking on the link, they will be able to browse through a larger number of jobs. If the job matches their criteria, they can look for further details by clicking on the link. In the current scenario, they need to click on all the links to find out the details and then decide which leads to lots of missed opportunities. Increased interest from the jobseekers will encourage more employers to post jobs, thus perpetuating a cycle of growth. 

Future Scope :

The model can be improved even further if we are able to provide tags based upon the generated labels. We can also add tags for Employment Type, Salary etc. With more granulated data, the need to navigate through multiple pages will reduce to just glancing at the search results and filtering out the ones that don’t fit the needs of the user. The advanced model can use our current model for it’s underlying logic. These steps will help Craigslist be a pioneer job hunt website.


