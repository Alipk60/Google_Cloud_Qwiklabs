# Google_Cloud_Qwiklabs

Learn to Earn 

******************************#***********************************
Internet of Things: Qwik Start

Overview
      
Cloud IoT Core is a fully managed service that allows you to easily and securely connect, manage, and ingest data from millions of globally dispersed devices. 
Cloud IoT Core, in combination with other services on Google Cloud IoT platform, provides a complete solution for collecting, processing, analyzing, and visualizing IoT data 
in real time to support improved operational efficiency.
      
Key concepts
To understand Cloud IoT Core, you should be familiar with the following concepts:

Internet of Things (IoT)

A collective term for the physical objects that are connected to the internet and can exchange data without user involvement.

Device

A "Thing" in the Internet of Things - a processing unit that is capable of connecting to the internet and exchanging data with the cloud. Devices are often called "smart devices" or "connected devices". They communicate two types of data: telemetry and state.

Telemetry

All event data (for example, measurements about the environment) sent from devices to the cloud. Telemetry data sent from a device to the cloud is called "device telemetry event" data. You can use Google Cloud Big Data Solutions to analyze telemetry data.

Device state

An arbitrary, user-defined blob of data that describes the current status of the device. Device state data can be structured or unstructured, and flows only in the device-to-cloud direction.

Device configuration

An arbitrary, user-defined blob of data used to control or change a device's state. Configuration data can be structured or unstructured, and flows only in the cloud-to-device direction.

Device registry

A container of devices with shared properties. You "register" a device with a service (like Cloud IoT Core) so that you can manage it (see the next item in this list).

Device manager

The service you use to monitor device health and activity, update device configurations, and manage credentials and authentication.

MQTT

An industry-standard IoT protocol (Message Queue Telemetry Transport). MQTT is a publish/subscribe (pub/sub) messaging protocol.

Components
The main components of Cloud IoT Core are the device manager and the protocol bridges:

A device manager for registering devices with the service, so you can then monitor and configure them.
Two protocol bridges (MQTT and HTTP) that devices can use to connect to Google Cloud.
Device telemetry data is forwarded to a Cloud Pub/Sub topic, which can then be used to trigger Cloud Functions. You can also perform streaming analysis with Cloud Dataflow or custom analysis with your own subscribers.

The following diagram summarizes the service components and the flow of data:

2b51c11919b21ede.png

This hands-on lab shows you how to use Cloud Console to create a Cloud IoT Core device registry and register a device. It also shows you how to run a sample to connect a device and publish device telemetry events.


******************************#***********************************
