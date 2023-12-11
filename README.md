# Patient Management System and Diet Plans

This system is designed to allow nutritionists to manage patients and assign them specific diet plans.

## Classes Used

### 1. Patient

- **Attributes:**
    - `patientId` (int): Patient identifier.
    - `name` (String): Patient name.
    - `age` (int): Patient age.
    - `weight` (double): Patient weight.
    - `height` (double): Patient height.
    - `preexistingConditions` (String): Pre-existing patient conditions.

- **Principal Methods:**
    - `registerPatient():` Displays a message when a patient is registered.
    - `updatePatientInfo():` Displays a message when updating patient information.
    - `deletePatient():` Displays a message when deleting a patient.
    - `getPatientId():` Returns the patient ID.
    - `toCsvString():` Converts patient information to CSV format.

### 2. Dietitian

- **Attributes:**
    - `dietitianId` (int): Nutritionist identifier.
    - `name` (String): Name of nutritionist.
    - `specialty` (String): Specialty of the nutritionist.

- **Principal Methods:**
    - `registerDietitian():` Displays a message when a dietitian is registered.
    - `manageDietitian():` Displays a message when managing a dietitian.
    - `toCsvString():` Converts dietitian information to CSV format.

### 3. DietPlan

- **Attributes:**
    - `planId` (int): Diet plan identifier.
    - `patient` (Patient): Patient associated with the diet plan.
    - `dietitian` (Dietitian): Nutritionist associated with the diet plan.
    - `dailyCalories` (double): Daily calories of the diet plan.
    - `macronutrientDistribution` (String): Macronutrient distribution of the diet plan.
    - `specificRecommendations` (String): Specific diet plan recommendations.

- **Principal Methods:**
    - `createDietPlan():` Displays a message when a diet plan is created.
    - `adjustDietPlan():` Displays a message when adjusting a diet plan.
    - `setPatient():` Assigns a patient to the diet plan.
    - `setDietitian():` Assigns a dietitian to the diet plan.
    - `getPatient():` Returns the patient associated with the diet plan.
    - `getDietitian():` Returns the dietitian associated with the diet plan.
    - `toCsvString():` Converts diet plan information to CSV format.

### 4. Meal

- **Attributes:**
    - `name` (String): 
    - `macronutrients` (String): 
    - `calories` (double): 
    - `timeOfDay` (String):

- **Principal Methods:**
    - `toCsvString():` Converts meal information to CSV format.

### 5. DemoCsv

    - Utility class for reading from and writing to CSV files.

- **Principal Methods:**
    - `writeCsv(String filePath, List<String> lines):` Writes lines to a CSV file.
    - `readCsv(String filePath):` Reads data from a CSV file.

### 6. Main

    - Main class for running the console-based user interface.

- **Principal Methods:**
    - `main(String[] args):` Entry point of the program.
    - `dietitianMenu(Scanner scanner, Dietitian dietitian):` Displays the menu for a logged-in dietitian.
    - `registerNewPatient(Scanner scanner, Dietitian dietitian):` Handles the registration of new patients.
    - `logIn(Scanner scanner):` Handles the login process for dietitians.
    - `registerNewDietitian(Scanner scanner):` Handles the registration of new dietitians.
 
### Author
    - `David Felipe Suarez Porres`


