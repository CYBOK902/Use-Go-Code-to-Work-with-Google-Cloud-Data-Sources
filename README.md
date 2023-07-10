# Use-Go-Code-to-Work-with-Google-Cloud-Data-Sources
Use Go Code to Work with Google Cloud Data Sources
************************************************************************************

Task - 1
gcloud auth list
gcloud config list project
export PROJECT_ID=$(gcloud info --format="value(config.project)")
go version
git clone https://github.com/GoogleCloudPlatform/DIY-Tools.git
gcloud firestore import gs://$PROJECT_ID-firestore/prd-back

Task 2. Review the Google Cloud Data Drive source code
package main
import (
    "log"
    "net/http"
    "os"
    "github.com/GoogleCloudPlatform ... /gcpdatadrive"
)

Task 4. Compile and run Google Cloud Data Drive application in Cloud Shell
cd ~/DIY-Tools/gcp-data-drive/cmd/webserver
go build -mod=readonly -v -o gcp-data-drive
./gcp-data-drive

Task 5. Test the application in your browser
export PROJECT_ID=$(gcloud info --format="value(config.project)")
export PREVIEW_URL=https://8080-cs-5571c71b-5f06-4f71-af62-f7f2700ee930.ql-asia-southeast1-wlry.cloudshell.dev/
echo $PREVIEW_URL/fs/$PROJECT_ID/symbols/product/symbol


Task 5. Test the application in your browser
export PROJECT_ID=$(gcloud info --format="value(config.project)")
export PREVIEW_URL=[REPLACE_WITH_WEB_PREVIEW_URL]
echo $PREVIEW_URL/fs/$PROJECT_ID/symbols/product/symbol
