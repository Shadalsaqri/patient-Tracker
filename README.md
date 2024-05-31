# patient-Tracker
class Patient:
    def __init__(self, patient_id, name, age, condition):
        self.patient_id = patient_id
        self.name = name
        self.age = age
        self.condition = condition

    def __str__(self):
        return f"ID: {self.patient_id}, Name: {self.name}, Age: {self.age}, Condition: {self.condition}"

class PatientTracker:
    def __init__(self):
        self.patients = []

    def add_patient(self, patient):
        self.patients.append(patient)

    def view_patients(self):
        for patient in self.patients:
            print(patient)

# Sample usage
if __name__ == "__main__":
    tracker = PatientTracker()
    tracker.add_patient(Patient(1, "Ali Ahmed", 30, "Flu"))
    tracker.add_patient(Patient(2, "Sarah Mohammed", 25, "Cold"))
    tracker.view_patients()
    
