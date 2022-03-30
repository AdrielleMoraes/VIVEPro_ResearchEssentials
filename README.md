# VIVEPro_ResearchEssentials

This repository contains a set of useful scripts to set up the HTC Vive Pro headset on windows. Additionally, it aims data collection saving all perfomance and physiological metrics to txt files.

This Repository was created to supply scripts for the [VivePro headset](https://www.vive.com/eu/product/vive-pro/) while developing in [Unity version 2020.3.19f1](https://unity3d.com/unity/whats-new/2020.3.19).

Before using this code, it is important to set up the development environment correctly. Dependencies to run this script include:

1. [Viveport SDK](https://developer.vive.com/resources/viveport/sdk/documentation/english/viveport-sdk/integration-viveport-sdk/unity-developers/) on Unity
2. Steam VR to run code on the headset
3. Vive [SRAnipal SDK](https://vr.tobii.com/sdk/develop/unity/getting-started/vive-pro-eye/)

## Data related to Eye movement: 
All gaze data is recorded at 120 Hz
| Variable Type | Description | 
| --- | --- |
| `Timestamp` | Timestamp in ms of when sample was recorded |
| `Pupil Diameter` | Combined (left and right) pupil diameter. Measured in mm. |
| `Gaze Direction X` | Combined gaze direction on the X axis |
| `Gaze Direction Y` | Combined gaze direction on the Y axis |
| `Gaze Direction Z` | Combined gaze direction on the Z axis |
| `Gaze Origin X` | Combined gaze origin on the X axis |
| `Gaze Origin Y` | Combined gaze origin on the Y axis |
| `Gaze Origin Z` | Combined gaze origin on the Z axis |
| `Head Direction X` | Head direction on the X axis |
| `Head Direction Y` | Head direction on the Y axis |
| `Head Direction Z` | Head direction on the Z axis |
| `Head Origin X` | Head origin on the X axis |
| `Head Origin Y` | Head origin on the Y axis |
| `Head Origin Z` | Head origin on the Z axis |

## Data related to Perfomance: 
All performance data is capture once for each frame.
| Variable Type | Description | 
| --- | --- |
| `Timestamp` | Timestamp in ms of when sample was recorded |
| `Left Controller push button` | Boolean variable with the status of the button |
| `Left Controller trigger button` | Boolean variable with the status of the button |
| `Right Controller push button` | Boolean variable with the status of the button |
| `Right Controller trigger button` | Boolean variable with the status of the button |

All data is saved to a txt file inside the project's main folder.
