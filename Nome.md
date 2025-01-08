# LibertyWalk-Java

---

## Statement

You must create a system model for a garage specializing in JDM cars, which has detailed information about the cars, their parts, types of modifications, among others. You will need to use relationships between classes in a complex way.

---

### Class responsibilities:

#### Car:
- **Attributes**:
	- Model
	- Manufacturer
	- Year
	- Engine
	- Modifications
	- Car Parts
- **Methods**:
	- Add mods
	- Remove mods
	- Description

#### Engine:
- **Attributes**:
	- Type
	- Power
- **Methods**:
	- Description

#### Car parts
- **Attributes**:
	- name
	- type
	- originality
- **Methods**:
	- Description

#### Modifications
- **Attributes**:
	- Type
	- Details
- **Methods**:
	- Description

#### Garage
- **Attributes**:
	- Cars
	- max Capacity
- **Methods**:
	- Add cars
	- Remove cars
	- List cars