# Muthu Kumar Photography CMS

Flask photography portfolio with an Admin Upload Dashboard.

## Local

python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app/app.py

Portfolio: http://127.0.0.1:5000
Admin: http://127.0.0.1:5000/admin/login

Default login: admin / muthu123

Change the password before production using ADMIN_PASSWORD.

## Deployment

This project includes render.yaml for Render. Uploaded media and SQLite need persistent storage. For a large production portfolio, move media to Cloudinary/S3-compatible storage.


## Render note
This version stores the SQLite database and uploaded media under `/opt/render/project/src/data`, which is the attached persistent disk mount. Do not change the disk mount to the source-code `app` directory.
