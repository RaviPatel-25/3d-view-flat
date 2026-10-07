# House 3D Flask Viewer

## 1. Put your GLB file here

Copy your model exactly to:

    static/models/house.glb

So the final structure is:

    house_3d_flask/
    ├── app.py
    ├── requirements.txt
    ├── README.md
    ├── templates/
    │   └── index.html
    └── static/
        └── models/
            └── house.glb       <-- YOUR FILE HERE

## 2. Install Flask

Windows:

    py -m pip install -r requirements.txt

If `py` doesn't work:

    python -m pip install -r requirements.txt

## 3. Start the server

    python app.py

You should see something like:

    Running on http://127.0.0.1:5000
    Running on http://192.168.x.x:5000

## 4. Open on your phone

Make sure the phone and PC are connected to the SAME Wi-Fi.

Find your PC's local IPv4 address using:

    ipconfig

Look for:

    IPv4 Address

For example:

    192.168.1.10

Then open on the phone:

    http://192.168.1.10:5000

Do NOT use 127.0.0.1 on the phone.

## Controls

Phone:
- Drag the screen = look around
- ▲ = forward
- ▼ = backward
- ◀ = left
- ▶ = right

PC:
- Mouse drag = look
- W / Arrow Up = forward
- S / Arrow Down = backward
- A / Arrow Left = left
- D / Arrow Right = right

## Important

The project uses Three.js from jsDelivr CDN. You do not need to download Three.js manually.

The only model file you need to supply is:

    static/models/house.glb
