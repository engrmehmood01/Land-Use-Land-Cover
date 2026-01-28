# Dynamic World LULC (Pakistan) | Google Earth Engine

Land Use / Land Cover (LULC) mapping for Pakistan using **Google Dynamic World V1** in **Google Earth Engine (GEE)**.  
This script mosaics Dynamic World classification for a selected time window, clips it to Pakistan boundary, visualizes with a custom palette, adds a boundary overlay, and builds a map legend.

## Output
- Dynamic World **label** band (classes 0–8)
- Map visualization with custom color palette
- Pakistan boundary outline
- Legend panel (bottom-left)

## Dataset
- **Dynamic World V1**: `GOOGLE/DYNAMICWORLD/V1`

## Classes (Dynamic World label)
| Value | Class |
|------:|-------|
| 0 | Water |
| 1 | Trees |
| 2 | Grass |
| 3 | Flooded vegetation |
| 4 | Crops |
| 5 | Shrub & Scrub |
| 6 | Built-up |
| 7 | Bare ground |
| 8 | Snow & Ice |

## Requirements
- Google Earth Engine account
- Pakistan boundary as a FeatureCollection asset (or replace with any ROI)

> Note: This repo uses an ROI asset:
`projects/metric-426111/assets/Pakistan_Boundary`

If you don’t have this asset, replace it with:
- a public boundary dataset (USDOS/LSIB_SIMPLE/2017), or  
- your own uploaded boundary

## How to Run
1. Open the Earth Engine Code Editor: https://code.earthengine.google.com/
2. Create a new script and paste the code from:
   `dynamic_world_lulc_pakistan.js`
3. Click **Run**
4. Adjust:
   - `startDate`
   - `endDate`
   - `roi` (boundary/area of interest)
   - visualization palette if needed

## Export (Optional)
The export-to-Drive block is included but commented.
Uncomment it if you want to export the classified raster.

## Author
Mehmood Ahmad  
Data Analyst | GIS & Remote Sensing | Google Earth Engine | Python & Excel Workflows
