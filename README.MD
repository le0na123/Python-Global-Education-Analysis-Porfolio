<style>
h1{
    text-align: center;
    text-transform: uppercase;
}
h3{
    font-size: 25px;
}
div.container{
    width: 50%;
    margin: auto;
}
pre{
    padding: 10px;
    border-radius: 5px;
     position: relative;
}
code {
    font-family: 'Courier New', Courier, monospace;
    background-color: #f4f4f4;
    padding: 2px 4px;
    border-radius: 3px;
    font-size: 17px;
}
.copy-btn {
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 5px 10px;
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
.copy-btn:focus {
    outline: none;
}
p{
    line-height: 35px;
    font-size: 15px;
}
</style>

<h1 style="">Global Education Analysis</h1>
<div class="container">
    <h3>Import libraries</h3><br>
        <pre><code id="code-block">
            import pandas as pd<br>
            import numpy as np<br>
            import matplotlib.pyplot as plt<br>
            import seaborn as sns
        </code>
    <h3>Data preperation</h3>
        <pre><code>df = pd.read_csv('data/Global_Education.csv')</code></pre>
        <p>
            * Countries and Areas: Name of the countries and areas.<br>
            * Latitude: Latitude coordinates of the geographical location.<br>
            * Longitude: Longitude coordinates of the geographical location.<br>
            * OOSR_Pre0Primary_Age_Male: Out-of-school rate for pre-primary age males.<br>
            * OOSR_Pre0Primary_Age_Female: Out-of-school rate for pre-primary age females.<br>
            * OOSR_Primary_Age_Male: Out-of-school rate for primary age males.<br>
            * OOSR_Primary_Age_Female: Out-of-school rate for primary age females.<br>
            * OOSR_Lower_Secondary_Age_Male: Out-of-school rate for lower secondary age males.<br>
            * OOSR_Lower_Secondary_Age_Female: Out-of-school rate for lower secondary age females.<br>
            * OOSR_Upper_Secondary_Age_Male: Out-of-school rate for upper secondary age males.<br>
            * OOSR_Upper_Secondary_Age_Female: Out-of-school rate for upper secondary age females.<br>
            * Completion_Rate_Primary_Male: Completion rate for primary education among males.<br>
            * Completion_Rate_Primary_Female: Completion rate for primary education among females.<br>
            * Completion_Rate_Lower_Secondary_Male: Completion rate for lower secondary education among males.<br>
            * Completion_Rate_Lower_Secondary_Female: Completion rate for lower secondary education among females.<br>
            * Completion_Rate_Upper_Secondary_Male: Completion rate for upper secondary education among males.<br>
            * Completion_Rate_Upper_Secondary_Female: Completion rate for upper secondary education among females.<br>
            * Grade_2_3_Proficiency_Reading: Proficiency in reading for grade 2-3 students.<br>
            * Grade_2_3_Proficiency_Math: Proficiency in math for grade 2-3 students.<br>
            * Primary_End_Proficiency_Reading: Proficiency in reading at the end of primary education.<br>
            * Primary_End_Proficiency_Math: Proficiency in math at the end of primary education.<br>
            * Lower_Secondary_End_Proficiency_Reading: Proficiency in reading at the end of lower secondary education.<br>
            * Lower_Secondary_End_Proficiency_Math: Proficiency in math at the end of lower secondary education.<br>
            * Youth_15_24_Literacy_Rate_Male: Literacy rate among male youths aged 15-24.<br>
            * Youth_15_24_Literacy_Rate_Female: Literacy rate among female youths aged 15-24.<br>
            * Birth_Rate: Birth rate in the respective countries/areas.<br>
            * Gross_Primary_Education_Enrollment: Gross enrollment in primary education.<br>
            * Gross_Tertiary_Education_Enrollment: Gross enrollment in tertiary education.<br>
            * Unemployment_Rate: Unemployment rate in the respective countries/areas.<br></p>
     <h3>Chage name of some columns</h3>
     <pre><code>df.rename(columns={'Countries and areas': 'Countries'}, inplace=True)</code></pre>

       
</div>


