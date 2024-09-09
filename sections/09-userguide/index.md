---
title: User guide
has_children: false
nav_order: 10
---

# User Guide
# User Guide for PlantAI

This guide explains how to use **PlantAI** from a user’s perspective, assuming the application has been successfully deployed.

## Accessing PlantAI

Once the application is deployed, you can access it via your browser by navigating to the provided URL (e.g., `https://plantai.vercel.app`). **PlantAI** is designed to be used both online and offline, so once you've visited the site, you can continue using it without an internet connection.

## Using PlantAI to Identify Plants

1. **Upload a Plant Image**:
   - On the homepage, you will see a drag-and-drop area or a button to **Select an Image**. 
   - You can either drag an image of a plant into the designated area or click the button to select an image from your device.

2. **Choose Plant Location**:
   - Below the image upload section, select whether the plant is **Indoor** or **Outdoor** by choosing the appropriate radio button.
   - This selection helps **PlantAI** provide accurate care instructions.

3. **Submit the Image**:
   - Once you’ve uploaded the image and selected the plant location, click the **Submit** button.
   - **PlantAI** will process the image using AI and identify the plant.
   
4. **View Plant Information**:
   - After processing, the app will display the plant’s common name, scientific name, watering schedule, and care instructions.
   - If the image does not contain a plant, the app will notify you with a message like "Plant not recognized."

5. **Save Plant Data**:
   - **PlantAI** stores your plant identification history locally in your browser. You can revisit the app and see the list of previously identified plants and their care instructions.

## Managing Plant Care

### Viewing Past Responses
- Scroll down on the homepage to see the **Saved Plant Responses** section. This section contains the plants you’ve previously identified, along with their watering schedule and care instructions.

### Watering Reminders
- If you have allowed notifications, **PlantAI** will send you reminders based on the watering schedule of the identified plants. These notifications will appear even if you are not actively using the app, helping you take care of your plants.

## Offline Usage

**PlantAI** supports offline usage thanks to its service worker:
- Once you’ve visited the site, the necessary files will be cached, allowing you to access and use **PlantAI** without an internet connection.
- You can view previously saved plant responses and continue identifying new plants even when offline. The new identification requests will be processed as soon as you regain an internet connection.

## Additional Features for debbuging

- **Clear Storage**: If you want to reset the saved plant data, you can click the **Clear Storage** button on the homepage. This will remove all locally saved plants from your browser.
- **Enable Notifications**: If you haven’t enabled notifications yet, you can click the **Enable Notifications** button to start receiving watering reminders for your plants.

---

By following this guide, you’ll be able to fully utilize **PlantAI** to identify plants, track their care, and receive reminders for watering, ensuring your plants remain healthy and well-cared for.
