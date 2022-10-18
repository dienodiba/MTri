# MTri
Magnetotelluric Inversion with Unstructured Triangular Mesh 

## Description
MTri is a two-dimensional finite element magnetotelluric inversion code that supports an unstructured mesh of triangular electrical resistivity elements. The unstructured mesh is handy for dealing with complex geometries. For example, the undulation of surface topography can sometimes influence MT data. This topographic effect must be corrected by accurately modeling the topography in the modeling domain, or it leads to an incorrect interpretation of the structure. For that, the unstructured mesh is preferred over the simple structured mesh. Besides, the unstructured mesh can accommodate local refinement to improve modeling accuracy. Common in practice is the refinement of the elements surrounding observation stations.

## Features

The code implements:
- Node-based finite element formulation for triangular elements
- Regularized least-squares objective function
- Model space Gauss-Newton minimization algorithm
- Reciprocity method for assembling the sensitivity matrix

The code can invert:
- apparent resistivity
- phase
- vertical magnetic field transfer function
- inter-station horizontal magnetic field transfer function

## Example

![ForGithub](https://user-images.githubusercontent.com/65894100/196236640-85baaff2-f9d6-4a2f-b547-07a57d6d1342.png)
