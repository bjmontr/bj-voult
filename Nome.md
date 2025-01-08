# Exercicio-Montadora-Java

---

## Enunciado

Você deve criar um modelo de sistema para uma garagem especializada em carros JDM, que tenha informações detalhadas sobre os carros, suas peças, tipos de modificações, entre outros. Você precisará usar relacionamentos entre as classes de forma complexa.

---

### Responsabilidades da classe:

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