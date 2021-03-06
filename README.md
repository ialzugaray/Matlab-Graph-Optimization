This is a matlab code package for **nonlinear least squares optimization**, based on the well-known concept--**Factor Graph**. 

# Organization
1.	Data: store the data to be processed
2.	Factor: the edge and node 
3.  g2o_files: core, provide the main framework of the nonlinear least squares
4.  Math: provide the mathematical operation like so3_exp,...
5.  auxilliary: others
6.  Geometry: some operations on geometry such as triangulation
7.  Doc: two tutorial notes

# Document
1. A tutorial for Optimization on Manifold
2. A tutorial for Graph Optimization

# Customization
This code allows users to define new variable nodes and new factors/edges/cost functions.
The framework is reorganized with necessary warnings for the extension of the new node and new edge.

1. When the new node is defined, the information needs to be given in the “GetNodeTypeDimension”, “SetNodeDefaultValue” and “update_state”.
2. When the new edge is defined, the information needs to be given in “GetFactorX_format” and “GetEdgeTypeDimension”.

# Examples for study/use
1. When you want to perform the estimation for 2D RGBD case, just run “Example_VictoriaPark.m”.
2. When you want to perform the estimation for 3D vision case, just run “Vision_Example_Small.m”.


# Updates
1. Any variable can be fix in the process of optimization
2. Schur decomposition has been added
3. Levenberg-Marquart and Powell's Dogleg have been added
4. A novel IMU factor for VINS has been added
5. Parallax vision factors have been added
6. VisionTest fator has been added 
