# AliCloud-Recording-File-Recognition
A VBO providing integration with AliCloud Recording File Recognition API

## Usage
The asset provides the following methods. 

* **Send Recognition Request**
* **Get Recognition Result**

Further details about the API including input/output parameters can be found at <https://www.alibabacloud.com/help/doc-detail/90727.htm?spm=a2c63.p38356.b99.38.33fa1d87rWIg5u>

## Configuration

* Download or clone this repository. Extract the *.bprelease file* and import it into your Blue Prism environment
* Create an account at <https://us.alibabacloud.com/>
* Activate Intelligent Speech Interaction service. Follow steps as outlined in <https://www.alibabacloud.com/help/doc-detail/69835.htm?spm=a2c63.p38356.879954.3.4d2537b77GE7PK>
* Create an Access Key. Follow steps as outlined in <https://www.alibabacloud.com/help/doc-detail/53045.htm>
* Enter the AccessKeyId and SecretAccessKey into the "Blueprism AlibabaCloud Short Sentence Recognition" in credential manager
* Create an App Key. Follow steps as outlined in <https://www.alibabacloud.com/help/doc-detail/71936.htm?spm=a2c63.p38356.879954.5.29e77eedEpUufM> Check the format and audio sampling rate of your recording file. Select a project that has an appropriate scenario and model in the console based on your business scenario.
* Store the recording file in Object Storage Service (OSS). If the access permission of the file is public, directly obtain the OSS URL of the file. <https://www.alibabacloud.com/help/doc-detail/39607.htm?spm=a2c63.p38356.879954.6.64fe37a7xsNwIY> If the access permission of the file is private, use the SDK to generate an OSS URL that has a validity period. <https://www.alibabacloud.com/help/doc-detail/31952.htm?spm=a2c63.p38356.879954.7.64fe37a7xsNwIY>
* Download dll zip from <http://sdk-release2.oss-cn-hangzhou.aliyuncs.com/dllfiles/aliyun-net-sdk-core-1.1.9.zip> and extract aliyun-net-sdk-Core.dll at path C:\Program Files\Blue Prism Limited\Blue Prism Automate
* Send a recording file recognition request using "Send Recognition Request" action.If the request is successful, the recording file recognition server returns the task ID, which can be used to query the recognition result.
* Call action "Get Recognition Result" to get the response JSON


## Help

If issues are encountered, please submit a new issue on the Issues tab for this repository:

https://github.com/blue-prism/AliCloud-Recording-File-Recognition/issues

