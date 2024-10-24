## <h1 style="font-size: 36px; font-weight: bold;">Project #2: Visualize Data using Amazon QuickSight (Beginner)</h1>

<p style="font-size: 18px; font-weight: bold;">Overview</p>
<p style="font-size: 16px;">
This project is designed to help you learn how to create visualizations using Amazon S3 and Amazon QuickSight. 
You'll be working with a dataset of 50,000 best-selling products from Amazon.com, stored in a CSV file, 
and we'll use QuickSight to generate meaningful graphs and insights from the data. By the end of the project, 
you will be able to create bar charts, pie charts, and other visual representations of data.
</p>

<p style="font-size: 18px; font-weight: bold;">Step #1: Download the Dataset</p>
<p style="font-size: 16px;">
To get started, you need to download two files: the "Amazon Bestseller Dataset" CSV file and the "manifest.json" file. 
These files are necessary for connecting Amazon S3 with QuickSight.
</p>

<ol style="font-size: 16px;">
    <li>Navigate to the <strong>2-s3-quicksight</strong> section where these files are available for download.</li>
    <li>Click on the "raw" button for both files (CSV and JSON), and press <strong>Control+S</strong> to save them to your computer.</li>
</ol>

<p style="font-size: 18px; font-weight: bold;">Step #2: Store the Dataset in Amazon S3</p>
<p style="font-size: 16px;">
Amazon S3 (Simple Storage Service) is where we will store the dataset. QuickSight will retrieve the data from this location for visualization.
</p>

<ol style="font-size: 16px;">
    <li>Go to the <strong>Amazon S3</strong> console by searching for "S3" in the AWS Management Console.</li>
    <li>Click the <strong>"Create Bucket"</strong> button. A bucket is a container that stores your files in S3.</li>
    <li>Give your bucket a name (e.g., <strong>"my-amazon-dataset"</strong>). Keep all other settings at their default values and click "Create."</li>
    <li>Once your bucket is created, open it and upload the <strong>CSV</strong> and <strong>manifest.json</strong> files you downloaded earlier.</li>
    <li>After uploading, locate the CSV file URL in S3 (by clicking on the file) and update the <strong>"manifest.json"</strong> file to include this URL under the data URL section.</li>
</ol>

<p style="font-size: 18px; font-weight: bold;">Step #3: Connect S3 Bucket with Amazon QuickSight</p>
<p style="font-size: 16px;">
In this step, we'll link Amazon S3 with Amazon QuickSight. QuickSight is a tool that helps you create charts and dashboards from large datasets.
</p>

<ol style="font-size: 16px;">
    <li>Open the <strong>AWS Management Console</strong> and search for <strong>Amazon QuickSight</strong>.</li>
    <li>If you don’t already have an account, sign up for a free trial (select the <strong>Enterprise edition</strong> for full features).</li>
    <li>Once you're in QuickSight, choose <strong>Amazon S3</strong> as your data source and check the box next to your S3 bucket.</li>
    <li>Enter the URL of the <strong>"manifest.json"</strong> file that points to your CSV data in S3 and connect to QuickSight.</li>
    <li>When prompted, select the <strong>"Interactive Sheet"</strong> option, which allows you to start working with your dataset and visualizing the data.</li>
</ol>

<p style="font-size: 18px; font-weight: bold;">Step #4: Create Visualizations</p>
<p style="font-size: 16px;">
Now that your data is connected to QuickSight, it's time to create visualizations.
</p>

<ol style="font-size: 16px;">
    <li>On the left, you'll see the fields from your dataset (like product name, category, sales, etc.). Start by dragging fields into the visualization pane.</li>
    <li>For example, drag <strong>"Product Category"</strong> and <strong>"Total Sales"</strong> to create a bar chart of the most popular categories on Amazon.</li>
    <li>You can customize each visualization by filtering data (e.g., showing only certain categories) or changing graph types (bar charts, pie charts, line charts, etc.).</li>
    <li>Feel free to explore different visualizations and experiment with sorting, grouping, and formatting options available in QuickSight.</li>
</ol>

<p style="font-size: 18px; font-weight: bold;">Files in the Repository</p>
<ul style="font-size: 16px;">
    <li><strong>Amazon Bestseller Dataset (CSV):</strong> Contains the data for 50,000 best-selling products on Amazon.</li>
    <li><strong>manifest.json:</strong> Provides schema and connection details for linking the dataset in S3 to QuickSight.</li>
</ul>

<p style="font-size: 18px; font-weight: bold;">Conclusion</p>
<p style="font-size: 16px;">
By completing this project, you now know how to upload datasets to Amazon S3 and create interactive data visualizations in Amazon QuickSight. You can use these skills to analyze large datasets and present insights in a visually appealing way. Experiment with different charts and try using other datasets for more practice!
</p>
