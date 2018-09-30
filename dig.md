<!-- TITLE: CURL domains and grab output -->
<!-- SUBTITLE: A quick summary of curl -->

# Script

CURL domains and grab output

#!/bin/bash

urls=( http://gdurl.com/PNo6 http://gdurl.com/PNo6/_/604ee6c49cd6b722880998c957ff5c82 http://gdurl.com/3Grf http://gdurl.com/3Grf/_/f392f3ef068b97f90a47f12dfa8afa79 http://gdurl.com/VJks http://gdurl.com/RTRhm http://gdurl.com/mGzk http://gdurl.com/GW6l http://gdurl.com/9YRz http://gdurl.com/BefQ http://gdurl.com/HwYl http://gdurl.com/n_sE http://gdurl.com/7m0s http://gdurl.com/dBcH http://gdurl.com/uZD8 http://gdurl.com/AOiu http://gdurl.com/Z1Ha http://gdurl.com/3Grf http://gdurl.com/PNo6 http://gdurl.com/F7_X http://gdurl.com/hyVC http://gdurl.com/jI9t http://gdurl.com/kwbx http://gdurl.com/bRkA http://gdurl.com/ThwI http://gdurl.com/BvwS http://gdurl.com/ClMy http://gdurl.com/0M2n http://gdurl.com/Twwr http://gdurl.com/Ojwq http://gdurl.com/2jzZ http://gdurl.com/JAQC http://gdurl.com/V4fz http://gdurl.com/vT3O http://gdurl.com/ZQLu http://gdurl.com/sfY5 https://gdurl.com/qRaT https://gdurl.com/flLs https://gdurl.com/nJ0Z https://gdurl.com/jxRN )

for i in ${urls[@]}; do
  echo $i >> dataout
  echo `curl ${i}` >> dataout
  echo "------------------------------------------------------------------------" >> dataout
done
# Commonds (Common + Commands)

$ curl -sIL