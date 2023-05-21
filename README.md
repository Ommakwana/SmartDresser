# Smart Dresser


<div style="text-align: justify">
Welcome to Smart Dresser, an AI-powered outfit selector designed to make your shopping experience **faster, easier, and safer**. Our product is the result of years of development aimed at addressing the challenges of traditional shopping and improving the overall customer experience.

With Smart Dresser, you can try on clothes virtually without the need for physical contact, **reducing the risk of exposure to COVID-19**. Our system uses advanced technology, including machine learning, image processing, and body posture detection, to provide **personalised outfit recommendations based on your preferences and body type**. By detecting your body posture and facial features, Smart Dresser offers tailored outfit suggestions that fit your style and complement your body shape.

We are committed to creating innovative solutions that solve real-world problems and improve people's lives. Our product not only provides **convenience and safety benefits** but also **reduces environmental impact and saves time**. We believe that shopping should be an enjoyable experience, and our goal is to provide a **real-
time, interactive shopping experience to the user**.
</div>



# Features & Technologies Used


|          **Features**         |        **Technologies**       |
| :-----------------------:| :-----------------------:|
| Virtual try-on without physical contact |   Image Processing    |
| Personalized outfit recommendations based on preferences and body type | Recommendation System |
| Tailored outfit suggestions that fit style and complement body shape |  Body Posture Detection |
| Reduces environmental impact and saves time | Data processing & Data visualization |


# Block Diagram 

![](https://github.com/Ommakwana/SmartDresser/blob/main/Images/Diagram.png)

***

**<p> User Login Page </p>**
---

<div style="text-align: justify">


The user login page serves as the entry point for users to access the application. 
It provides a secure authentication process, ensuring that only authorized users can proceed further. 
The login page is designed using **Tkinter**, a Python GUI library, to create an intuitive and user-friendly interface. 
The graphical elements and layout of the page are designed using **Figma**, a popular design tool. 
The login page acts as the initial step for users to access the various features and functionalities of the application.
</div>


**<p> Pickle Generation </p>**
---

<div style="text-align: justify">

Pickle generation involves the creation and storage of serialized Python objects. 
In this context, it plays a crucial role in capturing and preserving the relevant data for subsequent processes. 
The application utilizes the **RPi** module to establish a connection with the connected camera and initiate the recording process. 
The recorded data is then serialized using the **pickle** module, allowing efficient storage and retrieval of the captured information. 
This block lays the foundation for further image processing and analysis.
</div>


**<p> Face Detection</p>**
---

<div style="text-align: justify">

Face detection is a key component of the system, responsible for identifying and localizing human faces within the recorded video or images. 
Through the utilization of pre-built machine learning models, this block enables the system to accurately detect and extract facial features from the captured data. 
The processed output from this block serves as an input for subsequent stages, such as **skintone detection** and **virtual try-on**, providing crucial information for personalized clothing recommendations.
</div>


**<p> Body Pose Detection</p>**
---

<div style="text-align: justify">

Body pose detection is another integral part of the system, which focuses on analyzing the body position and pose of individuals in the recorded video or images. 
Leveraging machine learning algorithms, this block identifies the positions and orientations of various body joints, enabling the system to understand the user's body dimensions and proportions. 
The output from this block is utilized in subsequent stages for **size predecision** and **virtual try-on**, facilitating accurate clothing recommendations and visualization.
</div>


**<p> Skintone Detection</p>**
---

<div style="text-align: justify">

Skintone detection plays a vital role in the system's ability to provide personalized clothing recommendations. 
By analyzing the processed output from the **face detection** block , this block identifies the user's skintone. 
It utilizes machine learning techniques to determine the dominant color tones in the user's complexion, allowing for the selection of clothing items that complement their specific skintone. 
The information gathered from this block contributes to enhancing the accuracy and relevance of the subsequent clothing recommendation stage.
</div>


**<p> Size Predecision</p>**
---

<div style="text-align: justify">

Size predecision is a crucial step in ensuring that the recommended clothing items fit the user accurately. 
By leveraging the **body pose detection** results (2.3), this block determines the user's body measurements, such as height, shoulder width, and waist size. 
These measurements are then used to estimate the appropriate sizes for different clothing items, ensuring a better fit and reducing the need for returns or exchanges. 
**Size predecision** significantly improves the overall user experience by offering personalized size recommendations.
</div>

**<p> Apparel Selection</p>**
---

<div style="text-align: justify">

Apparel selection allows users to choose their preferred clothing items from a wide range of options. 
The system presents the user with a curated selection of clothes based on their **skintone**, **body measurements**, and **style preferences**. 
This block facilitates an intuitive and interactive interface where users can browse through various clothing options and select the ones they like. 
The chosen clothes are then stored for further processing and personalized recommendations.
</div>

**<p> Clothing Recommendations</p>**
---

<div style="text-align: justify">

The clothing recommendations block utilizes advanced algorithms and **machine learning** techniques to suggest personalized clothing items to the users. 
It takes into account the user's skintone, body measurements, and previous apparel selections to generate a tailored set of recommendations. 
By analyzing patterns, styles, and user preferences, this block helps users discover new clothing options that align with their individual tastes and enhance their overall shopping experience.
</div>


**<p> Virtual Try-On</p>**
---

<div style="text-align: justify">

The virtual try-on block enables users to visualize how selected clothing items would look on them before making a purchase. 
By utilizing **augmented reality** (AR) or **virtual reality** (VR) technologies, this block superimposes the chosen clothes onto a live video feed or uploaded images of the user. 
Users can see themselves virtually wearing the selected garments, allowing them to assess the fit, style, and overall appearance. 
This interactive and immersive experience empowers users to make more informed decisions and boosts their confidence in the chosen clothing items.
</div>


**<p> Checkout</p>**
---

<div style="text-align: justify">

The checkout block provides users with a seamless process to review and finalize their selected clothing items for purchase. 
Users can view a detailed list of the clothes in their shopping cart, including images, descriptions, sizes, and prices. 
They have the option to make any necessary modifications, such as adding or removing items, adjusting quantities, or applying discount codes. 
The checkout process incorporates secure payment gateways to ensure the confidentiality and safety of users' financial information. 
Once the purchase is confirmed, users receive an order summary and confirmation, marking the successful completion of their transaction.
</div>


**<p> Database Management</p>**
---

<div style="text-align: justify">

The database management block is responsible for **efficiently storing** and **managing** user data on both local and cloud storage systems. 
It ensures the secure storage and retrieval of user information, including login credentials, preferences, selected clothing items, and purchase history. 
By utilizing appropriate database management systems, this block allows for efficient data organization, indexing, and querying, ensuring smooth user interactions and seamless integration with other system components.
</div>


**<p> Offline Storage</p>**
---

<div style="text-align: justify">

The offline storage block focuses on preserving user data in a **local storage system**, ensuring accessibility and functionality even in the absence of an internet connection. 
It safeguards user information, including profiles, selected clothes, and purchase history, on the user's device. 
Offline storage enables users to continue using the application, reviewing their preferences, and making clothing selections even when offline. 
This block ensures a consistent and **uninterrupted user experience**, regardless of the availability of an internet connection.
</div>


**<p> Cloud Storage</p>**
---

<div style="text-align: justify">

The cloud storage block complements the offline storage system by securely storing user data on remote servers. 
It enables users to access their information from multiple devices and ensures data backup and synchronization across platforms. 
Cloud storage enhances the system's scalability, as it allows for seamless data sharing, collaboration, and synchronization between users and devices. 
It provides a reliable and efficient storage solution, reducing the risk of data loss and enhancing the overall user experience.
</div>


**<p> Store-Side Management</p>**
---

<div style="text-align: justify">
The store-side management block focuses on managing and organizing the backend processes and operations of the system from the perspective of the store or business. 
It includes various subblocks, such as inventory tracking and user **data management**, **data visualization**, and **bill generation**.
</div>


**<p> Inventory Tracking and User Data Management</p>**
---

<div style="text-align: justify">

The inventory tracking and user data management block enables efficient monitoring and management of the store's inventory and user-related information. 
It tracks the **availability** of different clothing items, updates stock levels in real-time, and ensures accurate representation of available products to users. 
Additionally, it **manages user data**, including preferences, purchase history, and account information. 
This block facilitates seamless inventory management and personalized user experiences, enhancing the efficiency and effectiveness of store-side operations.
</div>


**<p> Data Visualization</p>**
---

<div style="text-align: justify">

The data visualization block utilizes advanced visualization techniques and tools to present meaningful insights and analytics derived from user data and store-side operations. 
It provides visually appealing and interactive representations of data, such as sales trends, popular clothing items, user preferences, and customer behavior patterns. 
Data visualization helps store owners and administrators make informed decisions, identify market trends, optimize inventory, and improve overall business strategies.
</div>


**<p> Bill Generation</p>**
---

<div style="text-align: justify">

The bill generation block automates the process of **creating detailed bills** and **invoices for users' purchases**. 
It compiles relevant information, including selected clothing items, quantities, prices, applicable taxes, and discounts, into a structured format. 
The generated bills serve as documentation.
</div>






# Future Goal's

- Expand the range of clothing options.
- Improve accuracy of recommendations.
- Develop mobile application.
- Offer personalized size recommendations.
- Implementing social sharing features.

# Contributers

- [Harsh Shroff](https://github.com/HarshShroff)
- [Om Makwana](https://github.com/Ommakwana/Ommakwana)
- [Darshan Rathod](https://github.com/Darshanr5051)
- [Dishank Jogi](https://github.com/DishankJogi)





<p align="center">

<img align="center" src="https://img.shields.io/github/license/ommakwana/SmartDresser" />
<img align="center" src="https://img.shields.io/github/watchers/ommakwana/SmartDresser?style=social" />

</p>






