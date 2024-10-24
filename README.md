<h1 style="font-size: 36px; font-weight: bold;"> Visualize Data using Amazon QuickSight </h1>

<p><strong>Overview:</strong></p>
<p>
This project will guide you on how to use Amazon QuickSight, a powerful data visualization tool in AWS, to create graphs and reports from a large dataset. We will use a dataset of 50,000 best-selling products on Amazon, stored in a CSV file, and leverage Amazon S3 for storage. By the end of this project, you will be able to upload data to S3, connect it to QuickSight, and build insightful visualizations.
</p>

<h2 style="font-size: 24px; font-weight: bold;">Step #1: Download the Dataset</h2>
<p>First, you need to download the dataset that we will visualize. This dataset contains information on the top 50,000 best-selling products on Amazon.com.</p>

<ol>
    <li>
        Navigate to the <strong>2-s3-quicksight</strong> section (provided repository or link) to find the <strong>"Amazon Bestseller Dataset" CSV</strong> file and the <strong>"manifest.json"</strong> file.
    </li>
   
</ol>

<p><strong>What is manifest.json?</strong></p>
<p>
The <strong>manifest.json</strong> file is essential as it helps Amazon QuickSight understand where your dataset is located and how to access it. You will update this file with the correct S3 URL of your uploaded dataset in the following steps.
</p>

<h2 style="font-size: 24px; font-weight: bold;">Step #2: Store the Dataset in Amazon S3</h2>
<p>
Amazon S3 (Simple Storage Service) is where we will store the dataset before connecting it to QuickSight. Follow these steps to upload the files:
</p>

<ol>
    <li>
        Open the AWS Management Console, and search for <strong>Amazon S3</strong> in the search bar.
    </li>
    <li>
        Click <strong>"Create Bucket"</strong>. This bucket will act like a folder to store the dataset.
    </li>
    <li>
        Name your bucket (e.g., <strong>"my-amazon-dataset-bucket"</strong>), and leave all other settings as default. Click <strong>Create</strong>.
    </li>
    <li>
        Once the bucket is created, click on the bucket name and select the <strong>"Upload"</strong> button.
    </li>
    <li>
        Upload both the <strong>Amazon Bestseller Dataset CSV</strong> file and the <strong>manifest.json</strong> file that you downloaded in Step #1.
    </li>
    <li>
        After the files are uploaded, find the S3 URL of the <strong>CSV</strong> file. Copy this URL as you will need to update it in the <strong>manifest.json</strong> file.
    </li>
    <li>
        Open the <strong>manifest.json</strong> file on your computer in any text editor (like Notepad or VSCode). Replace the placeholder URL in the file with the actual S3 URL of your CSV file, then save it.
    </li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Step #3: Connect S3 Bucket with Amazon QuickSight</h2>
<p>
Now that your data is stored in Amazon S3 and the manifest file is updated, you need to connect Amazon QuickSight to your S3 bucket to start creating visualizations.
</p>

<ol>
    <li>
        In the AWS Management Console, search for and open <strong>Amazon QuickSight</strong>. 
    </li>
    <li>
        If you are using QuickSight for the first time, sign up for a free trial of the <strong>Enterprise edition</strong>. This trial is required to access the S3 data integration.
    </li>
    <li>
        Once inside QuickSight, click on <strong>"Manage data sources"</strong> on the dashboard and then click <strong>"New data set"</strong>.
    </li>
    <li>
        Select <strong>Amazon S3</strong> as your data source. You will be prompted to input the S3 URL for your <strong>manifest.json</strong> file (use the file with the correct S3 URL you updated in Step #2).
    </li>
    <li>
        Once the data source is connected, click on <strong>"Create data set"</strong>, and you will be asked to choose an analysis type. Select <strong>"Interactive Sheet"</strong> to begin building visualizations from the dataset.
    </li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Step #4: Create Visualizations</h2>
<p>
Now that the dataset is connected to QuickSight, you can start creating visualizations and explore different insights from the data. Here's how:
</p>

<ol>
    <li>
        In QuickSight, drag and drop fields from the dataset onto the visualization pane to create charts and graphs.
    </li>
    <li>
        For example, drag the <strong>"Product Category"</strong> field and <strong>"Total Sales"</strong> to create a bar chart showing the sales of different product categories.
    </li>
    <li>
        Customize the graph by using filters and sorting to focus on specific data points (e.g., highest-selling brands or top-rated products).
    </li>
    <li>
        You can also experiment with different chart types like <strong>bar charts, pie charts, line graphs</strong>, and more. QuickSight allows you to visually compare and analyze data in various ways.
    </li>
</ol>

<h2 style="font-size: 24px; font-weight: bold;">Files in the Repository</h2>
<ul>
    <li><strong>Amazon Bestseller Dataset (CSV):</strong> Contains the data of 50,000 best-selling products on Amazon.com.</li>
    <li><strong>manifest.json:</strong> Helps QuickSight locate and understand the dataset stored in S3.</li>
</ul>

<h2 style="font-size: 24px; font-weight: bold;">Conclusion</h2>
<p>
By following these steps, you will be able to store large datasets in Amazon S3 and connect them to Amazon QuickSight for powerful visualizations. These skills are valuable for working with large datasets and generating insights through data analytics.
</p>
<p>Feel free to experiment with other datasets and features in QuickSight to explore more advanced visualizations.</p>
