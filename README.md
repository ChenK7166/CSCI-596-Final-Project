# CSCI-596-Final-Project
### Team members: Kai Chen, Jingxin Zhang

## 1. Visualization
We simulate **Carbon Nanotube** using **Gromacs** and **jupyter notebook**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt.gif)

We also simulate **DNA**.

![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/dna.gif)


## 2. Prediction

Use Carbon Nanotubes Dataset from Kaggle.
This dataset contains 10721 initial and calculated atomic coordinates of the carbon nanotubes (CNTs)  


**Data Analysis:**  
- Sample:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/cnt_sample.JPG)

- Data Visualization using **plotly**:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_ex.gif)

- Visualize specific subset (n=11, m=2):  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/data_vis_11_2_ex.gif)

We would use neural network and some other machine learning models to predict Calculated atomic coordinates(u',v',w'), and compare their accuracy.


## 3. Performance Profile

Our team would use **cProfile** to analysis python program and uses **SnakeViz** and **VizTracer** to visualize the result.  

SnakeViz example:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/snakeviz_example.png)  

VizTracer example:  
![Alt Text](https://github.com/ChenK7166/CSCI-596-Final-Project/blob/main/Viztracer_example.png)  

## 4. Reference
Kaggle: <https://www.kaggle.com/inancigdem/carbon-nanotubes>
cProfile: <https://docs.python.org/3/library/profile.html>
SnakeViz: <https://jiffyclub.github.io/snakeviz/>
viztracer: <https://viztracer.readthedocs.io/en/latest/basic_usage.html>


