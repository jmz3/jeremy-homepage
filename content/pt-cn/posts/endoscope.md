+++
title = "ROS Driver for Fantronic Endoscopic Camera"
subtitle = "Software & Open-source"
author = "Jiaming Zhang"

date = "2025-02-01"
weight = 1
categories = ["technical","guide"]
tags = ["ROS","Endoscope","dVRK"]
#draft = "true"
plotly = "true"
image = "/images/xregi.png"


[[links]]
label = "Code"
url = "https://github.com/SMSL-Project/ros1-fantronics-endoscope"

+++

ROS1 image acquisition node for Fantronic/Geek Szitman endoscope camera. Supports USB connection. The camera can be purchased from Amazon from this [link](https://www.amazon.com/Inspection-Fantronics-Waterproof-Borescope-Adjustable/dp/B071HYRPND/ref=sr_1_1?dib=eyJ2IjoiMSJ9.zV1nqWnHEaSPdDiEHPP-RR0QeNAKRdKZrFqpH4skcsN3PcgYNpxxTd6n7FiPC8P5tZGjM3trSpj6Kf3AFw_GKZEuedP192EytwbsxPGmPA1LpuSVsZsCBGXyOL7zAXDaDGNGVcRh8U20rhtUt3EaU_U28Zv6Vmek0d28AWBRLqsjTfgybdPsb2lMmwTV2snLAotug0pMbluLOvZuIaJqgaEi97xg6jiTay9z4I9uhnA.GCo8pb43OOxapIJryI-bXsVdCcCdcgvRvehpc-ynycg&dib_tag=se&hvadid=651109964328&hvdev=c&hvexpln=0&hvlocphy=9007900&hvnetw=g&hvocijid=14768633232462871144--&hvqmt=e&hvrand=14768633232462871144&hvtargid=kwd-262769191435&hydadcr=977_1015116299&keywords=fantronics+endoscope&mcid=47abe76b718d31c78381e745b67076b3&qid=1763698904&sr=8-1).

With this ROS driver, you can easily use the endoscopic camera as wrist camera for da Vinci robot, who does not have native wrist camera support. 