<!DOCTYPE html>
<html>
<head>
    <h1>Concrete Strength Prediction</h1>
</head>
<body>
     <style>
        ul {
            list-style-type: square; /* Change bullet style */
        }
    </style>
<P>This project focuses on predicting the compressive strength of concrete based on its mix proportions and curing age. The dataset used consists of various features representing the ingredients of concrete and its curing age. The aim is to analyze the data, address multicollinearity, and build a reliable predictive model using machine learning techniques.
</p>
<br>
<h2>Features in the Dataset</h2>
<h3>The dataset consists of the following features:</h3>
<p>
<ul>
<li>Cement (kg/m³): Amount of cement in the mix.</li>
<li>Slag (kg/m³): Ground granulated blast-furnace slag.</li>
<li>Fly Ash (kg/m³): Pulverized coal ash.</li>
<li>Water (kg/m³): Quantity of water.</li>
<li>Superplasticizer (kg/m³): High-range water reducers</li>
<li>Coarse Aggregate (kg/m³): Amount of coarse aggregates.</li>
<li>Fine Aggregate (kg/m³): Amount of fine aggregates.</li>
<li>Age (days): Age of concrete curing.</li>
<li>Strength (MPa): Target variable representing the compressive strength.</li>
</ul>
</p>
<br>
<h2>Project Workflow</h2>
<ol>
    <h3><li>Data Loading and Preprocessing</li></h3>
    <ul>
        <li>The dataset is loaded and inspected for structure, types, and statistical summaries.</li>
        <li>There are no missing values, ensuring the data is clean and ready for analysis</li>
    </ul>
    <h3><li>Exploratory Data Analysis (EDA)</li></h3>
    <ul>
        <li><b>Heatmaps and Correlation:</b> Visualize relationships among features and the target variable.</li>
        <li><b>Feature Distributions:</b> Analyze data distributions to understand feature variability.</li>
        <li><b>Pairplot Analysis:</b> Detect potential multicollinearity and trends</li>
    </ul>
    <h3><li>Multicollinearity Detection and Removal</li></h3>
    <ul>
        <li><b>Variance Inflation Factor (VIF)</b> analysis identifies features contributing to multicollinearity.</li>
        <li>Features with high VIF are removed to improve the robustness of the model.</li>
    </ul>
    <h3><li>Data Splitting and Scaling</li></h3>
    <ul>
        <li>The dataset is split into training (80%) and testing (20%) subsets.</li>
        <li><b>StandardScaler</b> is applied to standardize features, ensuring they are on the same scale for improved model performance.</li>
    <ul>
    <h3><li>Building the Predictive Model</li></h3>
        <ul>
            <li>A <b>Linear Regression</b> model is implemented to predict compressive strength:</li>
                    <li>Trained using the processed training data.</li>
                    <li>Evaluated on the test set to measure model performance.</li>
        </ul>
    <h3><li>Model Evaluation</li></h3>
        <ul>
            <li>Model performance is assessed using metrics like <b>Mean Absolute Error (MAE), Mean Squared Error (MSE)</b>, and <b>R² score</b> to validate prediction accuracy.</li>
        </ul>
    </ol>
</body>
</html>


