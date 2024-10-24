<h1 style="font-size: 36px; font-weight: bold;">Project #2: Visualize Data using Amazon QuickSight (Beginner)</h1>

<p><strong>Overview:</strong></p>
<p>
This project is designed to help you learn how to create visualizations using Amazon S3 and Amazon QuickSight. 
You'll work with a dataset of 50,000 best-selling products from Amazon.com, stored in a CSV file. 
Using QuickSight, you'll generate meaningful graphs and insights from the data, like bar charts, pie charts, and more.
</p>

<h2 style="font-size: 24px; font-weight: bold;">Step #1: Download the Dataset</h2>
<p>
Download two important files: the <strong>"Amazon Bestseller Dataset" CSV</strong> file and the <strong>"manifest.json"</strong> file.
</p>

<ol>
    <li>Navigate to the <strong>2-s3-quicksight</strong> section where these files are available.</li>
    <li>Click on the "raw" button for both files, and use <strong>Control+S</strong> to save them to your computer.</li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Step #2: Store the Dataset in Amazon S3</h2>
<p>
Amazon S3 is where we will store the dataset. QuickSight will retrieve the data from this storage location.
</p>

<ol>
    <li>Go to the <strong>Amazon S3</strong> console.</li>
    <li>Click <strong>"Create Bucket"</strong>. A bucket is like a folder that stores files in S3.</li>
    <li>Give your bucket a name (e.g., <strong>"my-amazon-dataset"</strong>), and keep all other settings as default.</li>
    <li>Upload the <strong>CSV</strong> and <strong>manifest.json</strong> files into the bucket.</li>
    <li>Locate the S3 URL of your CSV file and update the <strong>"manifest.json"</strong> with this URL.</li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Step #3: Connect S3 Bucket with Amazon QuickSight</h2>
<p>
Now, connect your S3 bucket to Amazon QuickSight to start creating visualizations.
</p>

<ol>
    <li>Open <strong>Amazon QuickSight</strong> in the AWS Management Console.</li>
    <li>If you don't have an account, sign up for a free trial (choose <strong>Enterprise edition</strong>).</li>
    <li>Select <strong>Amazon S3</strong> as the data source and check your S3 bucket.</li>
    <li>Enter the URL of the <strong>manifest.json</strong> file and connect to QuickSight.</li>
    <li>Select <strong>"Interactive Sheet"</strong> to begin creating visualizations.</li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Step #4: Create Visualizations</h2>
<p>
Now it's time to create graphs using the data you've connected.
</p>

<ol>
    <li>Drag fields (like product name, sales, etc.) into the visualization pane in QuickSight.</li>
    <li>For example, drag <strong>"Product Category"</strong> and <strong>"Total Sales"</strong> to create a bar chart.</li>
    <li>Customize the visualizations using filters, sorting, and different chart types (e.g., pie charts, line graphs).</li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Files in the Repository</h2>
<ul>
    <li><strong>Amazon Bestseller Dataset (CSV):</strong> Contains the data for 50,000 best-selling products on Amazon.</li>
    <li><strong>manifest.json:</strong> Provides schema and connection details for linking the dataset to QuickSight.</li>
</ul>

<h2 style="font-size: 24px; font-weight: bold;">Conclusion</h2>
<p>
By the end of this project, you will be able to upload datasets to Amazon S3 and create interactive visualizations in QuickSight. 
These skills are valuable for analyzing large datasets and generating insightful reports. 
Feel free to experiment with other datasets to gain more practice!
</p>
