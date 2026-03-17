This repository contains the dataset used in the paper "DCMWAF-Net: Dual Cross-Modal Weighted Attention Feature Fusion Network for Multiscale Lunar Crater Detection".
# Overview

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
