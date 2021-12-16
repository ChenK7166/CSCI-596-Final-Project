# CSCI-596-Final-Project
### Team members: Kai Chen, Jingxin Zhang

## 1. Visualization
We simulate **Carbon Nanotube** using **Gromacs** and **jupyter notebook**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt.gif)
<p align="center">
    Figure 1 Carbon Nanotube Simulatio
</p>

We also simulate **DNA**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/dna.gif)
<p align="center">
    Figure 2 DNA Simulation
</p>

## 2. Prediction

Use Carbon Nanotubes Dataset from Kaggle.
This dataset contains 10721 initial and calculated atomic coordinates of the carbon nanotubes (CNTs)  


**Data Analysis:**  
- Sample:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt_sample.JPG)
<p align="center">
    Figure 3 Sample from dataset
</p>

- Data Visualization using **plotly**:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_ex.gif)
<p align="center">
    Figure 4 Data visualization
</p>

- Visualize specific subset (n=11, m=2):  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_11_2_ex.gif)
<p align="center">
    Figure 5 Subset visualization
</p>

**Prediction:**  
We use neural network and linear regression models to predict Calculated atomic coordinates(u',v',w') based on initial coordinates(u, v, w), and compare their accuracy. Linear regression uses the default parameters. Neural network set Learning rate to 0.0012, use Mean Squared Error as Loss function, set Adam as optimizer, use three hidden layers and 150 epochs. The change of loss with iteration is shown in figure 6.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/loss_over_iteration.png)
<p align="center">
    Figure 6 Loss over iteration
</p>
  
**Result:**  
Linear regression can achieve better results in all aspects by default  
<p align="center">
    Table 1 Comparsion in two models
</p>
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/result.jpg)  



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


