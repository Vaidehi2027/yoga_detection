# Yog-ood: Yoga se hi Hoga (Yoga Detection and Correction)
# Team Tech TrailBlazers
### [Figma Link](https://shorturl.at/ektyO)
### Inspiration
Yoga is important for a variety of reasons, encompassing physical, mental, and emotional well-being. Yoga involves a wide range of poses and movements that help improve flexibility, strength, balance, and posture. Regular practice can enhance muscle tone, joint mobility, and overall physical fitness. Yoga emphasizes deep breathing, mindfulness, and relaxation techniques. These practices can significantly reduce stress levels, calm the nervous system, and promote a sense of tranquility and inner peace. Through meditation and mindfulness, yoga helps clear the mind of clutter and promotes mental clarity. It can improve focus, concentration, and cognitive function, leading to better decision-making and problem-solving skills. Yoga encourages self-awareness and self-acceptance. It provides a safe space to explore and manage emotions, leading to improved emotional resilience and the ability to handle life's challenges more effectively. Yoga pose detection is important for several reasons, as it offers various benefits to individuals, practitioners, and the technology landscape. Yoga pose detection technology can provide real-time feedback on a user's pose alignment and execution. This personalized guidance helps practitioners improve their form and reduce the risk of injuries. With yoga pose detection, individuals can practice yoga at home or on the go without needing a physical instructor. This increases the accessibility of yoga practice, especially for those who may not have access to local yoga classes or instructors. Pose detection enables practitioners to practice yoga independently, allowing them to choose their practice time and pace. This independence fosters consistency and flexibility in their routine.

Accurate pose detection helps practitioners understand how their bodies should align in each pose. This correct alignment is crucial for maximizing the benefits of each pose while minimizing strain on muscles and joints. Real-time feedback from pose detection technology can alert practitioners when they are attempting poses with incorrect alignment. This reduces the risk of overexertion and injuries that could result from improper execution. Pose detection apps can track a user's progress over time, showing improvements in flexibility, strength, and pose mastery. This tracking can be motivating and encouraging for practitioners to continue their yoga journey.

### What it Does
‘Yoga pose: Detection, Classification, and Correction using ML’. Injuries due to wrong yoga poses can occur when practitioners perform poses with incorrect form, alignment, or excessive strain on the body. To prevent injuries, it is important for yoga practitioners to practice with a focus on proper alignment, gradual progression, and modifications when necessary. Not all can perform yoga with the presence of a qualified instructor at any suitable time. Thus, our system would allow users to perform yoga on their own independently at their convenient time, place and free of cost without the need for a qualified instructor. Our system would detect the pose; identify the particular yoga pose that is being performed and give feedback on it in real time. Doing a pose correctly enables achieving maximum health benefits and boosting the activeness of brain functionalities. We are attempting to build a system that detects, identifies, and corrects one’s Yoga posture, hence enabling people to exercise anywhere without the need for a physical trainer anytime and anywhere.

### How we Built it
Our solution is a free-of-charge real-time software that aims at helping people get a healthier lifestyle. The system training and development can be broken down into the following steps:
1. Importing Pre-trained weights from TensorFlow using 17 body parts such as left elbow, right elbow etc. will be defined by OpenPose. (OpenPose is a pose estimation library)
2. Creating a model which would identify the body parts using a live camera and form a skeletal image using the 17 different points (using OpenPose itself ) whose values will be stored every time a user is changing the body position
3. Training various correct Yoga postures into the model and storing the values of defined key points
4. The values will be 3D points derived from the skeleton formed from various correct yoga postures. The model would be a neural network model that uses CNN and libraries like PyQt for plotting the skeleton
5. Cross-check the values of each body part which would be captured by the camera with the original values of the Yoga postures and provide a result that includes the name of the posture and feedback about whether it is done correctly or not.

After the model has been created the workflow of the system would be:

1. The user would be in front of the camera doing some Yoga pose
2. The model would capture the values of different key points that the user’s posture is forming and plot a skeleton using those values and derive 3D points representing the user’s posture.
3. It will compare the points with all the postures it was trained on and provide a result including the type of pose, corrections if needed and any further remarks once it finds a match with an actual Yoga pose.

#### Challanges we ran into
Because of the time constraints, we could not develop a better front end with all the features that we thought of incorporating. But we would definitely improve the website with all the features.

### Accomplishments that we're proud of
The system would take details of a user including BMI, gender, age group, fitness goals and guide them on which exercises they should and should not do (which may help in refraining women from doing particular poses if they are menstruating or are expecting a baby).

1. It would provide users with personalized catalogs including instructions on how to do a particular pose according to their personal preferences and differentiate poses based on aspects they help in like flexibility, endurance, muscle strengthening, seasonal yoga poses, different yoga styles, workout of particular body parts and different intensity workout routines.
2. The system would work real time and hence help in not only identifying a particular yoga pose but also suggest on how to improve it; giving users a dynamic experience of self-paced exercise.
3. It would also focus on suggesting a proper diet according to the nutritional needs of a user.
4. It would enable users to create a custom workout routine in case they are professionals and are just using the software for consistency and self-training. Normal people: It can help people from any age group who are taking small steps to bring discipline and exercise hard to start a self-instructed yoga routine (particularly people who work jobs that does not include much physical activity) 2.Sportsman/athletes/professionals: It can be used by athletes to self-train themselves and customize their workout routines without the need of an instructor
5. For educational purposes: If integrated on larger scales it can be an educational and illustrative tool in schools and colleges for physical training or sport activities monitoring.
6. The system would be versatile enough to handle different body types, variations in lighting conditions, and various camera perspectives.
7. Practitioners would benefit from real-time feedback and guidance, helping them improve their posture forms and prevent injuries.
8. Our system would provide personalized corrections, and offer guidance to a larger audience through digital platforms

#### What we Learned
We learnt to work on various libraries of Python and tried various ML algorithms for detection and correctness. We learnt how to coordinate in a team and also work within the time boundaries. We also learnt how to design a website and incorporate it with a Jupyter notebook where we had written the ML algorithms for detection.

### What's Next for Yoga Detection and Correction
Using a depth camera to identify multiple bodies would probably solve the problem of multi-person pose estimation enabling multiple persons to use the system in a single frame.

1. Fine-tuning the model into identifying more Yoga asanas and enhancing features of the dataset (for eg. adding photos of individuals performing asanas outdoors too) to improve the accuracy of the model.
2. Moving forward the quality of OpenPose posture estimation by including adjustments by which it would perform well in cases of cover between individuals; cover between body parts or lost body parts.
3. The system could incorporate additional feedback mechanisms, such as audio and visual cues thereby providing users with even more information about their form and technique.
4. Adding security and privacy in the system to ensure that no data is saved or leaked without the permission of the user making it a reliable tool to exercise.
5. We can incorporate features like earning points or generating a progress report to motivate the user for exercise keeping in mind they are using a self-instructed yoga tool; this would not only terminate the need of an instructor but also ensure an uninjured yoga session.
6. Display the expected key points for the selected pose so users can align their body positioning with those key points rather than giving textual instructions which may be confusing at times.
7. Yoga is an ancient Indian practice so this system may help in popularizing this Indian art and reaching corners of the world due to its benefits and rich history.
