Standard Name Errors
====================

Overview
========

Message | Model/variable | Count | Example
 :--:  |  :--:  |  :--:  |  :--: 
['(3.3): Invalid standard\_name: tendency\_of\_surface\_snow\_and\_ice\_amount\_due\_to\_sublimation'] | ('EC-Earth3', 'Amon.sbl') | 158 | /badc/cmip6/data/CMIP6/CMIP/EC-Earth-Consortium/EC-Earth3/historical/r2i1p1f1/Amon/sbl/gr/v20190408/sbl\_Amon\_EC-Earth3\_historical\_r2i1p1f1\_gr\_187901-187912.nc
['(3.3): Invalid standard\_name: total\_water\_storage'] | ('CNRM-CM6-1-HR', 'Emon.mrtws'), ('IPSL-CM6A-LR', 'Emon.mrtws') | 20 | /badc/cmip6/data/CMIP6/HighResMIP/CNRM-CERFACS/CNRM-CM6-1-HR/highres-future/r1i1p1f2/Emon/mrtws/gr/v20190920/mrtws\_Emon\_CNRM-CM6-1-HR\_highres-future\_r1i1p1f2\_gr\_205001-205012.nc
['(3.3): Invalid standard_name: tendency_of_surface_snow_and_ice_amount_due_to_sublimation']
============================================================================================

```
	float sbl(time, lat, lon) ;
		sbl:standard_name = "tendency_of_surface_snow_and_ice_amount_due_to_sublimation" ;
		sbl:long_name = "Surface Snow and Ice Sublimation Flux" ;
		sbl:comment = "The snow and ice sublimation flux is the loss of snow and ice mass per unit area from the surface resulting from their direct conversion to water vapor that enters the atmosphere." ;
		sbl:units = "kg m-2 s-1" ;
		sbl:cell_methods = "area: time: mean" ;
		sbl:cell_measures = "area: areacella" ;
		sbl:history = "2019-03-05T17:18:25Z altered by CMOR: Reordered dimensions, original order: lat lon time." ;
		sbl:missing_value = 1.e+20f ;
		sbl:_FillValue = 1.e+20f ;
```

['(3.3): Invalid standard_name: total_water_storage']
=====================================================

```
	float mrtws(time, lat, lon) ;
		mrtws:long_name = "Total water storage in a grid cell" ;
		mrtws:units = "kg m-2" ;
		mrtws:online_operation = "average" ;
		mrtws:cell_methods = "area: mean where land time: mean" ;
		mrtws:interval_operation = "900 s" ;
		mrtws:interval_write = "1 month" ;
		mrtws:_FillValue = 1.e+20f ;
		mrtws:missing_value = 1.e+20f ;
		mrtws:coordinates = "" ;
		mrtws:comment = "ISBA-CTRIP total water storage (soil+canopy+snow+rivers+groundwater+floodplains; e.g. Decharme et al. 2018)" ;
		mrtws:standard_name = "total_water_storage" ;
		mrtws:description = "requested for C4MIP, OCMIP/OMIP, LUMIP, ScenarioMIP, DECK, DAMIP, GeoMIP, LS3MIP, ??" ;
		mrtws:history = "none" ;
		mrtws:cell_measures = "area: areacella" ;
```
