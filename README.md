- **polytope bias estimations** (PBE) for different input data domains:
  _given a collection of vectors (e.g. row vectors of a weight matrix), the PBE gives a bias vector_ $\alpha^\mathbb{K}$ _such that any ReLU-layer with bias_ $b\leq\alpha^\mathbb{B}$ _is injective on_ $K$
- **reconstruction formulas** for injective ReLU-layers

requirements
cvxpy==1.3.0
numpy==1.23.5
scipy==1.10.0
torch==2.0.0

To run ipynb file without warnings just write "solver=cp.ECOS" in terminal before running the code.

Important functions :
relu_inv and zcosz_inv computes the original input based on the cone of the facet it is present in.

Tested this method for a random poytope in R^3, icosahedron , tetrahedron.
