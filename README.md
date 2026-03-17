This repository contains the dataset used in the paper "DCMWAF-Net: Dual Cross-Modal Weighted Attention Feature Fusion Network for Multiscale Lunar Crater Detection".
# Overview
This project releases a multimodal annotated dataset for lunar craters with core information as follows:

1.Data source parameters:

Kaguya TC Morning: 48°W-69°W, 39°N-48°N, 61771×36602 pixels, 7.4031617 m/pixel, Equirectangular projection;

SLDEM2015: 180°W-180°E, 60°S-60°N, 184320×61440 pixels, 59.2252938 m/pixel, Equirectangular projection;

2.Annotated data: 85,878 manually labeled craters (diameter 0-13 km), with training set 59°W-69°W/45°N-48°N (59,665 craters) and test set 55°W-59°W/45°N-48°N (26,199 craters);

3.Generation process: Generated via research region selection (common area 48°W-69°W/39°N-48°N), data matching, image cropping & projection, and label matching;

4.Application scenarios: Supporting DCMWAF-Net model training, multimodal feature fusion research, and lunar crater catalog validation.
# Dataset
Crater_pro_v6

FID	Feature ID	Unique identifier for craters / Feature ID, integer type. Used to distinguish each individual crater in the dataset and avoid data confusion (e.g., FID1/FID2 correspond to different craters respectively).

x_coord	X Coordinate Longitude value of the crater (geographic coordinate), float type. West longitude is negative, east longitude is positive, unit: degree (°).

y_coord	Y Coordinate Latitude value of the crater (geographic coordinate), float type. North latitude is positive, south latitude is negative, unit: degree (°). Paired with x_coord to represent the geographic center of the crater.

Diam_km	Diameter in Kilometer Actual diameter of the crater, float type, unit: kilometer (km). Represents the effective diameter of the crater body.

tag	Label/Tag Classification / annotation label of the crater.

x_proj	X Projection Planar projected X value converted from the crater's geographic coordinates, float type, unit: meter (m) / kilometer (km).

y_proj	Y Projection Planar projected Y value converted from the crater's geographic coordinates, float type. Paired with x_proj to represent the center coordinate of the crater in the projected coordinate system.



Crater_pro_v6_data

A simplified version of Crater_pro_v6, retaining only the geographic longitude coordinate and diameter (the unit of diameter is meter (m)).
