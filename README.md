DCIT 313 Group Heptagon---Pest and Disease Detection Expert System

About This Project

This is our group project for DCIT 313. We built an Expert System that helps identify pests and diseases affecting crops. A user describes what they are observing on their crops (symptoms), and the system reasons through a knowledge base to tell them what pest or disease it likely is and what to do about it.

The system uses SWI-Prolog as the logic/reasoning engine and Python (via pyswip) as the interface the user interacts with.


Group Members

NAME  ---                    STUDENT ID  --     ROLE
Maame Esi Armah-Mensah –      22033196       Project Lead
Rebecca Anuoluwapo Ogunnubi-  11365448       Knowledge Engineers
Herbert Kojo Hayford –        22059074       Knowledge Engineers       
Bright Yaw Habada –           22047533       Programmers
Gabriel Ekow Eduful Ansah –   22018785       Programmers
Maxwell Adu –                 22232034       Programmers
Naeem Abdul-Aziz -            22117409       Programmers



How It Works

The user is shown a list of symptoms and selects the ones they can observe on their crops. The Python script takes those inputs and queries the Prolog knowledge base. Prolog matches the symptoms against its rules and returns a diagnosis along with a recommended course of action.

The intelligence of the system lives entirely in the Prolog rules — Python only handles the user interaction.

Project Structure


├── knowledge_base/
│   └── pest_disease_kb.pl    # All the facts and rules in Prolog
│
├── interface/
│   └── main.py               # The Python script the user runs
│
├── docs/
│   └── knowledge_engineering_report.pdf   # Our report
│
└── README.md


Running the System

Make sure you have SWI-Prolog and Python installed, then install pyswip:

bash
pip install pyswip


Then run:

bash
python interface/main.py


Course Info

Course: DCIT 313 – Introduction to Artificial Intelligence  
Group: Heptagon  

