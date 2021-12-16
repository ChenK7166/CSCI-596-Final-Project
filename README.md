# CSCI-596-Final-Project
### Team members: Kai Chen, Jingxin Zhang

## 1. Visualization
We simulate **Carbon Nanotube** using **Gromacs** and **jupyter notebook**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt.gif)
<center>Figure 1 Carbon Nanotube Simulation</center>

We also simulate **DNA**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/dna.gif)
<center>Figure 2 DNA Simulation</center>

## 2. Prediction

Use Carbon Nanotubes Dataset from Kaggle.
This dataset contains 10721 initial and calculated atomic coordinates of the carbon nanotubes (CNTs)  


**Data Analysis:**  
- Sample:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt_sample.JPG)
<center>Figure 3 Sample from dataset</center>

- Data Visualization using **plotly**:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_ex.gif)
<center>Figure 4 Data visualization</center>

- Visualize specific subset (n=11, m=2):  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_11_2_ex.gif)
<center>Figure 5 Subset visualization</center>

**Prediction:**  
We use neural network and linear regression models to predict Calculated atomic coordinates(u',v',w') based on initial coordinates(u, v, w), and compare their accuracy. Linear regression uses the default parameters. Neural network set Learning rate to 0.0012, use Mean Squared Error as Loss function, set Adam as optimizer, use three hidden layers and 150 epochs. The change of loss with iteration is shown in figure 6.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/loss_over_iteration.png)
<center>Figure 6 Loss over iteration</center>

**Result:**
Linear regression can achieve better results in all aspects by default
<center>Table 1 Comparsion in two models</center>
|                   | R-Squared | Mean Squared Error | Mean Absolute Error | train time | predict time |
|-------------------|-----------|--------------------|---------------------|------------|--------------|
| Linear Regression | 0.9995    | 4.4004             | 0.0019              | 0.0304     | 0.0005       |
| Neural network    | 0.9992    | 6.1290             | 0.0041              | 144.1802   | 0.2680       |


## 3. Performance Profile

At the beginning, our team wants to use **cProfile** to analyze python program and uses **SnakeViz** and **VizTracer** to visualize the logfile. However jupyter in the Colab do not support third party widgets. Therefore, we use

SnakeViz example:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/snakeviz_example.png)  

VizTracer example:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/Viztracer_example.png)  

## 4. Reference
Kaggle: <https://www.kaggle.com/inancigdem/carbon-nanotubes>  
cProfile: <https://docs.python.org/3/library/profile.html>  
SnakeViz: <https://jiffyclub.github.io/snakeviz/>  
viztracer: <https://viztracer.readthedocs.io/en/latest/basic_usage.html>  


