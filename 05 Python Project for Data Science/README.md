# Python Project for Data Science

**Project Overview**

In this project, We assume the role of a Data Scientist / Data Analyst working for a new startup investment firm that helps customers invest their money in stocks. The job is to extract financial data like historical share price and quarterly revenue reportings from various sources using Python libraries and webscraping on popular stocks. After collecting this data you will visualize it in a dashboard to identify patterns or trends. The stocks we will work with are Tesla, Amazon, AMD, and GameStop.

**Dashboard Analytics Displayed**

A dashboard often provides a view of key performance indicators in a clear way. Analyzing a data set and extracting key performance indicators will be practiced. Prompts will be used to support learning in accessing and displaying data in dashboards. Learning how to display key performance indicators on a dashboard will be included in this assignment. We will be using Plotly in this course for data visualization and is not a requirement to take this course.

In the Python for Data Science, AI and Development course you utilized Skills Network Labs for hands-on labs.

For this project you will use Skills Network Labs and Watson Studio. Skills Network Labs is a sandbox environment for learning and completing labs in courses. Whereas Watson Studio, a component of IBM Cloud Pak for Data, is a suite of tools and a collaborative environment for data scientists, data analysts, AI and machine learning engineers and domain experts to develop and deploy your projects.

**Review criteria**

There are two hands-on labs on Extracting Stock Data and one assignment to complete. You will be judged by completing two quizzes and one peer review assignment. The quizzes will test you based on the output of the hands-on labs. In the peer review assignment you will share and take screen shots of the outcomes of your assignment.

# Gamestop stock vs Tesla
Determining the price of a stock is complex; it depends on the number of outstanding shares, the size of the company's future profits, and much more.  An essential factor is the company's profit and growth of profits; if the company's profit is increasing, the stock price should increase.  If you suspect the company's profit increases, you should buy the stock as the stock should increase, But what happens if you think the stock price will decrease. 

Short selling is how you make money if the stock decreases. An investor borrows a stock, sells the stock, and then repurchases it to return it to the lender.  Typically stocks fall faster than they rise, so you can make a profit more quickly. Usually, experienced investors such as hedge funds partake in short selling. One problem is if the stock price increases, the investor can lose money.

Sometimes short sellers get it wrong; for example, Tesla.  A few years ago, many short sellers targeted Tesla. Then Tesla started becoming profitable, and profits were increasing; thus, the company stock went up. This was based on the companies performance, so the stock should continue to rise, and the short seller should sell the stock.  Recently shorted stocks can increase for reasons that are not based on fundamentals; this is less sustainable. 

Individual investors using the forum on the Reddit online community named WallStreetBets, started buying into shares of GameStop, a video and computer-game retailer losing money. The influx of demand caused GameStop shares to soar.  All this produced billions of dollars in losses for hedge funds who had sold the stock short. [
 1
] GameStop's share price should fall eventually, so the Hedge funds should hold on to the short positions. As a data scientist working for a hedge fund, you will extract the profit data for Tesla and GameStop and build a dashboard to compare the price of the stock vs the profit for the hedge fund.


[yfinance Library](https://author-ide.skills.network/render?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJtZF9pbnN0cnVjdGlvbnNfdXJsIjoiaHR0cHM6Ly9jZi1jb3Vyc2VzLWRhdGEuczMudXMuY2xvdWQtb2JqZWN0LXN0b3JhZ2UuYXBwZG9tYWluLmNsb3VkL0lCTURldmVsb3BlclNraWxsc05ldHdvcmstUFkwMjIwRU4tU2tpbGxzTmV0d29yay9sYWJzL3Byb2plY3QvWWZpbmFuY2VfcmVhZGluZy5tZC5tZCIsInRvb2xfdHlwZSI6Imluc3RydWN0aW9uYWwtbGFiIiwiYWRtaW4iOmZhbHNlLCJpYXQiOjE3MDA2NzQwOTZ9.Yxs0HynVMkt5mqqOKfgy1QnC8Sj-_LQ3MG6YnW1mFk8)

[Create IBMCloud account and Watson Studio instance](https://author-ide.skills.network/render?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJtZF9pbnN0cnVjdGlvbnNfdXJsIjoiaHR0cHM6Ly9jZi1jb3Vyc2VzLWRhdGEuczMudXMuY2xvdWQtb2JqZWN0LXN0b3JhZ2UuYXBwZG9tYWluLmNsb3VkL0lCTURldmVsb3BlclNraWxsc05ldHdvcmstUFkwMTAxRU4tU2tpbGxzTmV0d29yay9sYWJzL01vZHVsZSUyMDQvUFkwMTAxRU4tNC1MYWItTG9hZGluZyUyMERhdGElMjBhbmQlMjBWaWV3aW5nJTIwRGF0YS5tZCIsInRvb2xfdHlwZSI6Imluc3RydWN0aW9uYWwtbGFiIiwiYWRtaW4iOmZhbHNlLCJpYXQiOjE3MDA2NzEyOTV9.I0TzaX-7X15HjaB2dgPOrezAPs5GZJtlzvsjnND2qos)

[Add notebook to Watson Studio](https://author-ide.skills.network/render?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJtZF9pbnN0cnVjdGlvbnNfdXJsIjoiaHR0cHM6Ly9jZi1jb3Vyc2VzLWRhdGEuczMudXMuY2xvdWQtb2JqZWN0LXN0b3JhZ2UuYXBwZG9tYWluLmNsb3VkL0lCTURldmVsb3BlclNraWxsc05ldHdvcmstUFkwMTAxRU4tU2tpbGxzTmV0d29yay9sYWJzL0ZpbmFsTW9kdWxlX0NvdXJzZXJhL0lCTV9XYXRzb25fU3R1ZGlvX1Byb2plY3QubWQiLCJ0b29sX3R5cGUiOiJpbnN0cnVjdGlvbmFsLWxhYiIsImFkbWluIjpmYWxzZSwiaWF0IjoxNzAwNjcxMjUwfQ.b_0FdSS5d1LGsv2C-P_Htq797mjgmM3F4q7TFFFxcF4)

[Share your notebook from Watson Studio](https://author-ide.skills.network/render?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJtZF9pbnN0cnVjdGlvbnNfdXJsIjoiaHR0cHM6Ly9jZi1jb3Vyc2VzLWRhdGEuczMudXMuY2xvdWQtb2JqZWN0LXN0b3JhZ2UuYXBwZG9tYWluLmNsb3VkL0lCTURldmVsb3BlclNraWxsc05ldHdvcmstUFkwMjIwRU4tU2tpbGxzTmV0d29yay9sYWJzL3Byb2plY3QvU2hhcmUlMjB5b3VyJTIwbm90ZWJvb2subWQiLCJ0b29sX3R5cGUiOiJpbnN0cnVjdGlvbmFsLWxhYiIsImFkbWluIjpmYWxzZSwiaWF0IjoxNzAwNjY5OTcxfQ.fUA1khzXfoSIe4k_0eKo5NnG2ytwTl0rJyvUExWqevo)


# Certification and Batch
  
[<img align="right" width="400" src="https://images.credly.com/size/680x680/images/7d06faf8-c754-4ecd-8ab1-2115826b03c6/Python_Project_for_Data_Science.png">](https://www.credly.com/go/P5RlrZep)
<img  align="left"  alt="IBM" width="500" src="https://coursera-certificate-images.s3.amazonaws.com/HJKMTF52V7E2">
