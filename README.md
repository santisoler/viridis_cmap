# viridis
Simple PIP package to use viridis colormap in matplotlib 1.4

# How to install
Clone the repository:

    git clone https://www.github.com/santis19/viridis_cmap

then install the package with PIP:

    cd viridis_cmap
    sudo pip install .

Done! You are ready to use it.

# How to use viridis colormap
Just import the colormap in Python as follows:

    from viridis_cmap.cmaps import viridis

Example:

    import numpy as np
    import matplotlib.pyplot as plt
    from viridis_cmap.cmaps import viridis
    
    x = np.linspace(-1.0, 1.0, 101)
    x, y = np.meshgrid(x, x)
    z = x**2 + y**2
    
    
    plt.contourf(x, y, z, 15, cmap=viridis)
    plt.colorbar()
    plt.axes().set_aspect("equal")
    plt.show()
