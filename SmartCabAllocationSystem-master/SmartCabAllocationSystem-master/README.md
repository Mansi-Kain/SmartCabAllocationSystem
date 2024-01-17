# Smart Cab Allocation System

## Overview

**1. Administrative Cab Allocation Optimization:**

- **Objective:** Implement an algorithm to optimize cab allocation for trips, minimizing overall travel distance.
- **Tasks:**
    - Develop an algorithm suggesting the best cab based on proximity to the trip start location.
    - Integrate real-time location data for cabs and trip start locations.
    - Evaluate the algorithm's effectiveness in reducing travel distance and improving trip efficiency.

*Summary:* The primary focus is on creating an algorithm optimizing cab allocation for trips by considering the proximity of cabs to trip start locations. Real-time location data enhances algorithm precision, and rigorous testing ensures its effectiveness in minimizing travel distance.

**2. Employee's Cab Search Optimization:**

- **Objective:** Enhance the user experience for employees searching for cabs by suggesting nearby cabs in use.
- **Tasks:**
    - Utilize real-time data to display cabs engaged in trips and nearby to the employee's location.
    - Evaluate the system's effectiveness in providing quick and relevant cab suggestions for employees.

*Summary:* This aspect concentrates on improving the user experience by suggesting nearby cabs already in use. Real-time data ensures accurate suggestions, and evaluation guarantees the system's effectiveness in offering relevant suggestions promptly.

**3. Real-Time Location Data Integration:**

- **Objective:** Ensure seamless integration of real-time location data for cabs and trip start locations.
- **Tasks:**
    - Establish a robust system for real-time tracking of cab locations.
    - Integrate location data into the cab allocation algorithm for up-to-date suggestions.
    - Address potential challenges such as data latency or inaccuracies for system reliability.

*Summary:* The primary goal is to integrate real-time location data seamlessly, ensuring accuracy in suggestions. This involves establishing a robust tracking system, integrating data into the allocation algorithm, and addressing challenges for overall system reliability.

In summary, the project aims to create a comprehensive Smart Cab Allocation System optimizing cab allocation for efficient trip planning. It addresses administrative and employee perspectives, leveraging real-time location data for accuracy and effectiveness in cab suggestions. The project includes algorithm development, real-time data integration, and thorough testing and evaluation processes. Console logging provides feedback on algorithm results. User options include authentication, cost estimation, handling system failures, and more.

## Tech Stack Used

**1. Programming Language: C++**

- **Description:** The Smart Cab Allocation System's core is built in C++ for efficiency, performance, and versatility. C++ features facilitate robust system development, crucial for real-time processing and optimization.

**2. Object-Oriented Programming (OOP) Principles:**

- **Description:** OOP principles enhance code modularity, readability, and maintainability. The system structure revolves around key OOP concepts, ensuring encapsulation, inheritance, and polymorphism for modular components.

**3. Real-Time Data Integration:**

- **Description:** C++ features like classes and objects represent and manage cab and trip locations for seamless real-time data integration. OOP principles facilitate well-defined interfaces and interactions between objects for efficient real-time data handling.

**4. Algorithm Development:**

- **Description:** The cab allocation algorithm, implemented in C++, follows object-oriented design. Classes and structures represent trips and cabs, with methods encapsulating logic for optimal cab allocation. This modular approach enhances code clarity and reusability.

## Various Features

### Authentication

- The cab booking system employs a robust **static authentication mechanism** for secure access. Users authenticate with a unique username and password before booking a cab.

![Authentication Successful](https://github.com/Mansi-Kain/SmartCabAllocationSystem/blob/master/SmartCabAllocationSystem-master/SmartCabAllocationSystem-master/Images/img2.jpg)

![Authentication Failure](https://github.com/Mansi-Kain/SmartCabAllocationSystem/blob/master/SmartCabAllocationSystem-master/SmartCabAllocationSystem-master/Images/img1.jpg)

### Cost Estimation

- **Time Complexity and Space Complexity:**

The **findBestCab** operation's time complexity is O(n), where n is the number of cabs. Space complexity is O(n) for storing cab location data.

### Handling System Failure Cases

- The system is designed with high fault tolerance. In case of failures, it gracefully restarts.

### Object-Oriented Programming Language (OOPS)

- Abstraction, encapsulation, polymorphism, and modularization are fundamental OOP principles applied for code organization and flexibility.

![Abstraction and Encapsulation](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/ab782a07-4c98-4708-b3c7-82ea0b94fe33)

![Polymorphism](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/468f4b1a-c841-4c33-b937-054c0ced86b2)

### Trade-offs in the System

- UI Choice: A CLI-style UI was chosen for faster execution and less overhead.
- Performance vs. Accuracy: Opting for a simpler algorithm for quick cab allocation. A more complex algorithm could provide precise suggestions but might take longer.
- Consistency vs. Availability in Real-Time Data Integration: Strong consistency might impact system availability, especially in distributed scenarios.

### Error and Exception Handling

- Try-Catch blocks are implemented for critical operations, providing comprehensive error handling.

![Try-Catch Blocks](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/da78acac-2635-42aa-9c42-f6ddbfa1f16d)

- Comprehensive error handling ensures robust application performance with meaningful error messages.

![Comprehensive Error Handling](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/5c382ef1-1ba7-42cb-a818-df2b51ac07e2)

## Backend Installation

### Prerequisites

- clang version ≥ 14.0.6
- g++ ≥ 12.2.0

### Steps

1. **Clone the repository:**

```bash
git clone <>
cd SmartCabAllocationSystem
```

## Sample Output Screenshots

- Initial cab locations with latitude and longitude. Additional cabs can be added as needed.

![Cab Initial Locations](https://github.com/Mansi-Kain/SmartCabAllocationSystem/blob/master/SmartCabAllocationSystem-master/SmartCabAllocationSystem-master/Images/img3.jpg)

- User authentication and current location input. CLI tool prompts users for preferences.

![User Authentication and Input](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/f8e08ded-f199-44ad-9c98-875c0abdda53)

1. Display Nearby Cab Locations: Shows nearby cab allocations within a given limit.

![Display Nearby Cab Locations](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/981ba6a4-612b-4d2d-a5ab-18a70c480864)

2. Request a Cab - Displays the best cab and fare based on the current location, asking users if they want to book.

![

Request a Cab](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/0a1eb634-ecd2-4287-9d04-b9519060fb54)

![Cab Booking Confirmation](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/ce073460-a339-42fa-9e81-7f2aa2c21e3f)

3. Trip Completed - User and cab locations updated after the trip. New locations displayed and updated in the database.

![Trip Completed](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/da187049-7443-4b87-8dc0-aee22dd39b0d)

![No Ongoing Trip](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/128d764b-c0e5-4a9a-81d1-2c0258959196)

4.1 Get UserID, user location, and currently booked cab (cabID for valid trip, -1 for no current trip).

![Get User Information](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/7ebd174f-186c-4105-a718-76cbcb3cb1ab)

4.2 Cab location updated after the trip. Users can search for nearby cabs based on the new location.

![Cab Location Updated](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/315456dc-9850-497c-bc8b-bb30a7fa1501)

5. Exit the program from the CLI.

![Exit Program](https://github.com/aniket2405/SmartCabAllocationSystem/assets/64733221/709420ed-a8b6-441a-a316-e74876903263)
