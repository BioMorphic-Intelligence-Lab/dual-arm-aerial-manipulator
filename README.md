# Dual Arm Omnidirectional Aerial Manipulator mechanical design
This directory contains an export of the design files used to construct the Dual Arm Omnidirectional Aerial Manipulator. The design was made using Autodesk Fusion360, and the full exported archive can be found in `Fusion archive`. For 3D printed, STEP and STL exports are provided in case access to Fusion360 is not available. For lasercut/waterjetcut plate material (the body panels), the DXF is provided along with the STEP and STL.

ICRA paper: https://arxiv.org/pdf/2602.10703 \
Associated software repository: https://github.com/BioMorphic-Intelligence-Lab/manipulator_assisted_landing

## Part list
The design is divided into 6 mechanical sub-assemblies. Per sub-assembly a part list is provided.

### Rotor arm (4x/6x)
The standard edition uses 4 of this entire assembly, however the upper and lower body plates provide attachment points for another set, making this design into a hexarotor.
| **Part name**         | **Assembly** | **Part no.** | **Acquisition** | **Information**                    |
|-----------------------|------------------|--------------|-----------------|------------------------------------|
| Rotor Arm Clamp Upper | Rotor Arm        | RA-01a       | 3D print        |                                    |
| Rotor Arm Clamp Lower | Rotor Arm        | RA-01b       | 3D print        |                                    |
| Rotor Arm Rod         | Rotor Arm        | RA-02        | Buy/cut         | Outer diam 14 mm, inner diam 12 mm |
| Motor Bracket Upper   | Rotor Arm        | RA-03a       | 3D print        |                                    |
| Motor Bracket Lower   | Rotor Arm        | RA-03b       | 3D print        |                                    |
| Motor                 | Rotor Arm        | RA-04        | Buy             | E-MAX PRO 2814 830KV               |
| Propeller CW          | Rotor Arm        | RA-05a       | Buy             | GEMFAN 9045-3 CW                   |
| Propeller CCW         | Rotor Arm        | RA-05b       | Buy             | GEMFAN 9045-3 CCW                  |
|                       |                  |              |                 |                                    |

### Body
This assembly functions a bit like a bus, the structural attachment for all the other parts.
| **Part name**         | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition**      | **Information**                                               |
|-----------------------|------------|------------------|--------------|----------------------|---------------------------------------------------------------|
| Main Body Plate Upper | 2          | Body             | DB-01        | Buy/waterjet cutting | Find a supplier that allows cutting from DXF. Thickness 2 mm. |
| Main Body Plate Lower | 2          | Body             | DB-02        | Buy/waterjet cutting | Find a supplier that allows cutting from DXF. Thickness 2 mm. |
| Standoffs             | 8          | Body             | DB-03        | Buy                  | Length of 35 mm, threaded with M3.                            |
| Upper Cable Bridge    | 1          | Body             | DB-05        | 3D print             | Optional but handy.                                           |
| Lower Cable Bridge    | 2          | Body             | DB-06        | 3D print             | Optional but handy.                                           |
| ESC Bracket           | 1          | Body             | DB-07        | 3D print             | Advise to modify to fit your ESC.                             |
| Electronics Bracket   | 1          | Body             | DB-08        | 3D print             |                                                               |
| Leg                   | 4          | Body             | DB-09        | 3D print             |                                                               |
| Lidar/OF Plateau      | 1          | Body             | DB-10        | 3D print             |                                                               |
| Antenna Holder        | 1          | Body             | DB-12        | 3D print             |                                                               |
| Battery               | 2          | Body             | DB-15        | Buy                  | Any 2 identical 6S batteries should work.                     |

### Pivot Joint
| **Part name**       | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition** | **Information**                                                    |
|---------------------|------------|------------------|--------------|-----------------|--------------------------------------------------------------------|
| Sun Shaft           | 1          | Pivot Joint      | PJ-01        | Buy/lathe       | Use a strong material, I used steel but aluminium should work too. |
| Sun Gear            | 2          | Pivot Joint      | PJ-02        | 3D print        |                                                                    |
| Sun Bearing         | 2          | Pivot Joint      | PJ-03        | Buy             | Outer diam 42 mm, inner diam 20 mm, width 12 mm.                   |
| Inner Sun Spacer    | 1          | Pivot Joint      | PJ-04        | 3D print        |                                                                    |
| Outer Sun Spacer    | 2          | Pivot Joint      | PJ-05        | 3D print        |                                                                    |
| Planet Shaft        | 2          | Pivot Joint      | PJ-06        | Buy             | Solid aluminium axle diam 8 mm.                                    |
| Planet Gear         | 4          | Pivot Joint      | PJ-07        | 3D print        |                                                                    |
| Planet Bearing      | 8          | Pivot Joint      | PJ-08        | Buy             | Outer diam 16 mm, inner diam 8 mm, width 5 mm.                     |
| Inner Planet Spacer | 2          | Pivot Joint      | PJ-09        | 3D print        |                                                                    |
| Outer Planet Spacer | 4          | Pivot Joint      | PJ-10        | 3D print        |                                                                    |
| Drive Planet Gear   | 2          | Pivot Joint      | PJ-11        | 3D print        |                                                                    |
| Pivot Servo         | 2          | Pivot Joint      | PJ-12        | Buy             | Feetech ST3025                                                     |
| Pivot Clamp Lower   | 2          | Pivot Joint      | PJ-16        | 3D print        |                                                                    |
| Pivot Clamp Upper   | 2          | Pivot Joint      | PJ-17        | 3D print        |                                                                    |

### Shoulder Link (2x)
| **Part name**    | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition** | **Information**       |
|------------------|------------|------------------|--------------|-----------------|-----------------------|
| Ring Gear        | 1          | Shoulder Link    | SL-01        | 3D print        |                       |
| Shoulder Servo   | 1          | Shoulder Link    | SL-02        | Buy             | Feetech STS3250       |
| Ring Gear Flange | 1          | Shoulder Link    | SL-03        | 3D print        | Glue on the Ring Gear |




### Upper Arm Link (2x)
| **Part name**             | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition** | **Information**                                                                               |
|---------------------------|------------|------------------|--------------|-----------------|-----------------------------------------------------------------------------------------------|
| Upper Arm Link            | 2          | Upper Arm        | UA-01        | Buy/cut         | Best is to find a supplier that cuts to specified length. Outer diam 14 mm, inner diam 12 mm. |
| Elbow Servo               | 1          | Upper Arm        | UA-04        | Buy             | Feetech STS3235                                                                               |
| Servo Pulley              | 1          | Upper Arm        | UA-05        | 3D print        |                                                                                               |
| Elbow Hinge               | 1          | Upper Arm        | UA-07        | 3D print        |                                                                                               |
| Elbow Joint Spacer        | 1          | Upper Arm        | UA-08        | 3D print        |                                                                                               |
| Elbow Servo Bracket Left  | 2          | Upper Arm        | UA-09a       | 3D print        |                                                                                               |
| Elbow Servo Bracket Right | 2          | Upper Arm        | UA-09b       | 3D print        |                                                                                               |
| Shoulder Connector        | 1          | Upper Arm        | UA-10        | 3D print        |                                                                                               |
| Timing Belt               | 1          | Upper Arm        | UA-11        | Buy             | Used RS timing belt, modify Servo Pulley accordingly.                                         |
| Elbow Axle                | 1          | Upper Arm        | UA-12        | Buy/cut         | Aluminium axle (same as Planet Shaft).                                                        |
| Torsion Bracket           | 2          | Upper Arm        | UA-14        | 3D print        |                                                                                               |



### Forearm Link
| **Part name**     | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition** | **Information**         |
|-------------------|------------|------------------|--------------|-----------------|-------------------------|
| Forearm Link      | 1          | Forearm          | FA-01        | Buy/cut         | 14x12 carbon fibre tube |
| Elbow Pulley      | 1          | Forearm          | FA-02        | 3D print        |                         |
| Forearm Connector | 1          | Forearm          | FA-03        | 3D print        |                         |
| Elbow Flange      | 1          | Forearm          | FA-04        | 3D print        |                         |
| Elbow Spacer      | 1          | Forearm          | FA-05        | 3D print        |                         |
| Tube End          | 1          | Forearm          | FA-08        | 3D print        |                         |


### Electronics
| **Part name**       | **Amount** | **Sub-assembly** | **Part no.** | **Acquisition** | **Information**                                           |
|---------------------|------------|------------------|--------------|-----------------|-----------------------------------------------------------|
| ESC 4-in-1          | 1          | Electronics      | EL-01        | Buy             | T-Motor F55A Pro III 4in1                                 |
| Flight Controller   | 1          | Electronics      | EL-02        | Buy             | Holybro Pixhawk 6X                                        |
| Power Converter     | 1          | Electronics      | EL-03        | Buy             | Matek PM20S-2                                             |
| Flight Computer     | 1          | Electronics      | EL-04        | Buy             | Orange Pi 5B, but you can use any SBC like a Raspberry Pi |
| Servo USB-TTL board | 1          | Electronics      | EL-05        | Buy             | Feetech FE-URT-1 USB to TTL board                         |
| Receiver            | 1          | Electronics      | EL-06        | Buy             | FrSky X8R                                                 |
| Optical Flow        | 1          | Electronics      | EL-07        | Buy             | Holybro PMW3901                                           |
| Laser Rangefinder   | 1          | Electronics      | EL-08        | Buy             | ST VL53L1X Lidar Rangefinder                              |

## Tips


## License
