Model from http://dx.doi.org/10.5281/zenodo.13279

wget https://zenodo.org/record/13279/files/popc0-25ns.trr
wget https://zenodo.org/record/13279/files/popc25-50ns.trr
wget https://zenodo.org/record/13279/files/popc407.tpr
wget https://zenodo.org/record/13279/files/endCONF.gro

trjcat -f popc0-25ns.trr popc25-50ns.trr -o trajectory.xtc
mv popc407.tpr topol.tpr


cp ../../../../../MAPPING/mappingPOPCberger.txt mappingFILE.txt
cp /wrk/ollilas1/HGmodel/NMRlipids/lipid_ionINTERACTION/scratch/ffgmx2berger.hdb ./ffgmx2.hdb
cp /Users/osollila/NMRlipids/NmrLipidsCholXray/scratch/POPCberger/electronsBERGER.dat ./electronsLIPID.dat
