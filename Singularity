Bootstrap: docker
From: rocker/tidyverse:3.6.1

%labels
  Author Pawsey Supercomputing Centre
  Version 0.0.1

%startscript
  export R_PORT=${R_PORT:-"8787"}
  export R_ADDRESS=${R_ADDRESS:-"0.0.0.0"}
  
  rserver --www-port $R_PORT --www-address $R_ADDRESS --auth-none=1 --auth-validate-users=0
