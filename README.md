# HSCR
We seek to solve a critical problem faced by Ninjavan's sorting center. As-Is, the facility might experience delays and potential losses due to clogs caused by high influx of goods, coupled with a disorganised sorting process that makes it difficult to locate items. Our solution involves organising the warehouse to ensure efficient pallet placement, and implementing computer vision with AI to detect vacant spaces. This will provide decision makers with real-time information to facilitate transport of goods to either the sorting hub or backlog facility. By streamlining the sorting process, we can help Ninjavan save time, money, and provide a better experience for their consignees.

## Solution
Utilising computer vision to estimate warehouse capacity by to detecting empty boxed out spaces. Warehouse congestion status is displayed on a dashboard for the warehouse manager to monitor. Alerts/updates are also provided to drivers & ops personel in the event of the warehouse reaching capacity

## Assumptions
- Fixed position of camera (top-down)
- The staff will place the objects in the allocated grids
- Images are streamed to OBS (HuaWei Cloud)/S3 (AWS)

# Running our application
## Create virtual environment and install dependencies
- ```python -m venv venv```
- ```venv\scripts\activate```
- ```pip install -r yolov5/requirements.txt```

## Run frontend app on localhost
- ```cd hscr_frontend```
- ```npm install```
- ```npm run dev```
