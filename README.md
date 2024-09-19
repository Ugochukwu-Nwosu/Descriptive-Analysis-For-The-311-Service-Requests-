# Portfolio Project: Descriptive Analysis For The 311 Service Requests.

## Project Description:
Descriptive Analysis of Abandoned Non-Recyclables Service Requests

## Project Title:
Improving Waste Management: Analyzing Service Requests for Abandoned Non-Recyclables in Vancouver

## Objective:
This project will conduct a descriptive study on ‘Service Requests: Abandoned Non-recyclable Items’ in Vancouver. The analysis is intended to provide an overview of the critical patterns of service requests and discover trends and issues that will enhance the service for waste management in the city, especially about non-recyclable waste.

## Methodology:

![311 Service Requests drawio](https://github.com/user-attachments/assets/e58f0b0e-64d9-4077-a1cf-8f7a3f70ab8c)

## Dataset From Vancouver Open Data Portal:

![2023Datasets](https://github.com/user-attachments/assets/936de101-485e-4da2-9b7a-d2c84bd2e9fb)
![2024Dataset](https://github.com/user-attachments/assets/480095a0-be6b-4788-a884-19f6bb92ea53)

The data involves services made through the 3-1-1 system of Vancouver between the years 2023 and 2024. The key features of the dataset are:
Request ID: A code assigned to every service request made.
Request Date: The date and time of request implies the time when the request was made
Request Type: Nature of service request type (mainly targeted on “Abandoned Non-Recyclables”)
Request Location: Describe where the reported items were abandoned.
Response Time: The amount of time it took to respond to the request
Status: Whether the request is done or still in process
Neighborhood: The specific neighborhood within the catchment area of Vancouver from which the request can be made.
Reporting Channel: This indicates how the request was made and reported (phone, internet, among others).

## The Data Pipeline

![Pipeline1](https://github.com/user-attachments/assets/204e3260-75c4-4e7d-8673-2d09bf9a4e6d)
![Pipeline2](https://github.com/user-attachments/assets/21e895b7-f6ad-4fea-8535-36266c9f8041)
![Pipeline3](https://github.com/user-attachments/assets/29ec44e3-2596-4cac-a8ff-ecd016ecc649)
![Pipeline4](https://github.com/user-attachments/assets/5a045729-ac70-4491-b458-07e1ab00b017)

### Data Collection and Preparation:
	
This process involves gathering the necessary dataset from Vancouver’s Open Data Portal, explicitly focusing on 3-1-1 service requests related to "Abandoned Non-Recyclables—Small Case." The data ingestion process moves the prepared datasets into the operational environment. It loads them into the target locations of Amazon S3 and Google Colab. Pandas reads it into a data frame for subsequent cleaning, ensuring the data is ready for descriptive analysis. 

### The DAP Design and Implementation On AWS Cloud

Data Ingestion:
![311 Ingest1](https://github.com/user-attachments/assets/077a476a-c1ff-4f70-bb48-c694a0ee0718)
![Ingest2](https://github.com/user-attachments/assets/cc389615-ca02-43d7-aa68-59ccebe47476)

Data Storage:
![Data Storage](https://github.com/user-attachments/assets/da14dcd7-275e-4237-893e-bd9eae557836)

Data Cleaning:
![DataCleaning1](https://github.com/user-attachments/assets/07ca48db-b6ff-4f55-b095-8a449d446411)
![DatCleaning2](https://github.com/user-attachments/assets/0ed753b9-26fe-4839-a4dd-42b2f3129c12)

Data Pipeline Implementation:
![ETL1](https://github.com/user-attachments/assets/2982e985-decf-4190-b697-2ef924229d6e)
![ETL2](https://github.com/user-attachments/assets/448f5013-3a5c-4882-aa84-8c3b38e35554)

Data Analysis:
![DataAnalysis1](https://github.com/user-attachments/assets/d5a2885b-d322-4ad3-a100-4c5056341b79)
![DatAnalysis2](https://github.com/user-attachments/assets/72ecd5fe-64c2-4cf8-a301-697f6fb0f518)

Data Publishing:
![Data Publishing](https://github.com/user-attachments/assets/3f91fc23-7052-45a6-9776-754ed0604298)

Data Protection:
![DataProtection Through SS3 keys](https://github.com/user-attachments/assets/51bface9-f274-490c-a6d6-c18bcb1b2101)
![Data Protection](https://github.com/user-attachments/assets/1a363c21-b2c5-4d4a-b582-d03667b2f170)

Data Governance:
![DataGovernance](https://github.com/user-attachments/assets/0e304f79-dfaf-42cc-86a8-9239c400f1a0)

Data Monitoring:
![Data Monitoring 3](https://github.com/user-attachments/assets/76f04d62-7e2c-44db-b45b-fbfbd9b579ff)
![Data Monitoring](https://github.com/user-attachments/assets/05e9f3ef-a8df-4be0-a4d7-646e2396df04)
![DataMonitring](https://github.com/user-attachments/assets/358dac18-ad40-47f7-90d5-b1a0d0e7afce)

### The Descriptive Statistics

Now that the data is cleaned and combined, descriptive statistical analysis for 2023 and 2024 is done. This dataset provides a summary of the service requests made on non-recyclable items that are abandoned in Vancouver. There were a total of 1,317 service requests that were all addressed by the ENG – Sanitation Services. Among these, 1,305 requests (99%) can be considered closed, while 12 (1%) remain open, showing high closure rates. The total time it took to close a request was, on average, 6 days, 16 hours, and 22 minutes, which is efficient. For geographic distribution, Downtown received the most dominant number of requests at 265, while Grandview-Woodland and Strathcona ranked second and third, respectively. There were slightly fewer requests for other small neighborhoods, such as Arbutus Ridge and West Point Grey, with only a few cases. The most significant number of service requests were through the Mobile App, with 768 requests at 58%, followed by the Phone, with 303 requests at 23% and WEB, with 244 requests at 19%, with little entries from Social Media. The findings of this study show that engagement is high through digital means and service issues are efficiently resolved in critical neighborhoods. 

### The Data Visuaizations

#### Bar Plot for Service Requests by Department For 2023 and 2024
![Service_requests_by_Department](https://github.com/user-attachments/assets/b1a2e6ce-5674-44b5-9fe6-d4067d4e09bb)

#### Pie Chart for Service Request Status For 2023 and 2024
![Service_Request_Status](https://github.com/user-attachments/assets/7f99cb69-ce68-48ac-9bcc-241e28dc4edc)

#### Bar Plot for Service Requests by Local Area (Neighborhood) For 2023 and 2024
![Service_Requests_By_Local_Area](https://github.com/user-attachments/assets/2f6ea94c-bbff-4ccb-abc0-567721afd313)

![Service_Requests_By_LocalArea_2024](https://github.com/user-attachments/assets/9c9cf6dc-64ee-4d06-93a9-7818c92668f9)

#### Pie Chart for Service Requests by Channel For 2023 and 2024
![Service_requests_By_Channel](https://github.com/user-attachments/assets/f373310b-ad5b-44e1-ab89-3b72616addc3)

#### Histogram of Time to Close a Service Request For 2023 and 2024.
![TimeTo Close Request2023](https://github.com/user-attachments/assets/a701b01f-7c1c-45b2-8d64-7c24c9a00486)

![Time To Close Request 2024](https://github.com/user-attachments/assets/f99c3320-d07e-4646-9802-1b0463f497f5)

#### Heatmap of Service Requests by Local Area and Month (2023 & 2024)
![Service Requests From Both Datasets By Local Area and Month](https://github.com/user-attachments/assets/1068bce4-9e89-4553-a48e-ba63dd63b99a)


### Key Insights and Findings
This research explored the 311 service requests for the abandoned non-recyclables in Vancouver and here are the analysis that offers a range of insights and findings. Thus, these results reflect the effectiveness of services that provide garbage disposal in the city, the involvement of various districts, as well as the specified methods of reporting.

Peak Request Periods and Seasonal Trends
The heatmap of service requests by local area and month helps to identify the trends in the number of requests provided to different neighbourhoods in months. For example, Downtown is consistently among the top performers in the number of requests, probably explained by its population density and the many people passing through this area. This pattern indicates that maximum levels of abandoned non-recyclables occurs when more people are more likely to be in urban centres, for instance, after festivals or during festive seasons. Communities such as Grandview-Woodland and Strathcona also have high frequencies, which vary from month to year, suggesting that these places require more waste collection services at some time of the year. Awareness of such fluctuations will assist the city in planning and allocating resources to tackle waste management problems appropriately.

Neighborhoods with High Request Frequency
The bar plot representing service requests of non-recyclable materials by the local area unambiguously suggests that Downtown, Grandview-Woodland, and Strathcona are the most frequently reported neighbourhoods for abandoned non-recyclable reports. Such regions are usually urban, densely populated, and probably bear a higher level of public activity, which explains the higher report volume. At the same time, Arbutus Ridge, West Point Grey, and Kerrisdale have fewer cases, which could be explained by their less commercial and relatively sparsely populated. These differences in service requests suggest that urban places require more frequent and specific waste management services than residential ones.

Response Time Trends
The histogram of the time to close service requests shows that the average time taken to close a service request is 6 days, 16 hours, and 22 minutes; Vancouver’s waste management services are efficient. Still, there could be some differences concerning the neighbourhoods. For example, zones that receive more requests, such as Downtown, could take a little longer to close due to the increased workload, while zones with fewer requests will close faster. Knowledge about the specific request volume that draws a response will also help determine the bottleneck and areas that can be optimized to generate more response time. Furthermore, areas with many open requests will require more staff or efficient procedures for managing these cases.

 Completion Rates 
In the pie chart for the service request status, the ‘closed’ percentage is as high as 99%, while 1% was noted as ‘Open’. This high closure rate indicates that organizing Vancouver’s ENG - Sanitation services is prompt and effective in addressing any concerns from clients regarding the disposal of non-recyclable items. However, the 1% of open cases point to potential isolated problems in some neighbourhoods or reporting channels. It would be helpful to look at further factors contributing to the open requests and whether patterns indicate systemic issues with response time or difficulties processing specific categories of reports. This analysis could provide insights into recommendations for enhancing the open report or providing more resources to the repeat neighbourhoods for open requests.

Reporting Channel Preferences
The pie chart of service requests through the channels also shows that the most frequent reports made are through the Mobile App – 58%, Phone – 23% and Web – 19%. This reveals a high level of appreciation for digital reporting, which can be attributed to the optimum usage of mobile devices. From just two reports, it can be assumed that social media is not a very common channel for submitting service requests, possibly because of its classification or knowledge by the population. The high usage of mobile devices also indicates that the community is technically informed, so further advancements in reporting processes should be directed towards making online reporting more productive.
## Recommendations

To enhance response time to abandoned non-recyclable items, Vancouver should distribute more human power, resources and equipment in service demands areas such as Downtown, Grandview-Woodland, and Strathcona. It can be said that these areas receive more frequent reports and can have lower response times because of the increased flow of reports. To provide fast service, more personnel and waste collection vehicles should be provided in these areas, especially during busy hours. Also, it is possible to integrate smart resource distribution, which in real-time will allow setting priorities for requests in critical moments, for example, in the work zones that are quickly filling up with customers. 

Efficient awareness campaigns launched in areas with more significant numbers of abandoned items can effectively decrease the number of reports. Techniques that include educating the people in the neighbourhood and sensitization activities in collaboration with other community-based organizations will effectively ensure people dispose of their non-recyclable items properly (Kumar & Mittal, 2020). Besides awareness, increasing the waste bins across the areas and the number of recycling centres available will allow the residents to dispose of waste quickly. Advertising fines for improper waste disposal discourages individuals from depositing waste in the environment, encouraging proper waste disposal.

It is also important to refine the reporting system to increase the efficacy of the requests for service delivery. The authorities should encourage further reporting through the mobile app since it files 58% of reports and provides an enhanced and quicker means of reporting. Additional options for improving reporting will include simplifying the web reporting process for those who cannot use smartphones and considering the social networking option as one of the reporting tools. Incentivizing faster channels, such as the Mobile App, will help residents actively use these tools to increase the speed of request processing and its subsequent resolution.

