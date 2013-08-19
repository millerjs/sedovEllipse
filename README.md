
setup_call: ./setup Sedov -auto -2d -objdir mhd_sedovEllipse -noc +usm


- Adjusted the original sedov simulation to setup a pre-evolved shock front based on the spherical solution that was provided by Carlo.  The shock front was made elliptical by interpolating the solution and stretching the radii as a function of angle.

- Has been run in cylindrical coords as well as 2D cartesian.

- The fluid velocity along at the shock is constant in magnitude as a function of angle and is directed in the direction normal to the shock

- Shock front is proportional to r \sqrt{1 + \epsilon cos(\theta)^2} , where \epsilon is the eccentricity of the ellipse.