# Viết chương trình Flowchart bằng PlanUML

## Cú pháp cơ bản

```plant-uml
@startuml
start
:Action 1;
:Action 2;
if (Decision?) then (Yes)
  :Action 3;
else (No)
  :Action 4;
endif
:Final Action;
stop
@enduml
```

<figure><img src="../../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

## Ví dụ: Quy trình đăng nhập

```plant-uml
@startuml
start
:Input username;
:Input password;
if (Credentials valid?) then (Yes)
  :Display welcome message;
else (No)
  :Display error message;
endif
stop
@enduml
```

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>
