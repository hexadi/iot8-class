## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301018/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301018/model-01/sn-001
    - payload
        - {"temperature": 25.2}
        - {"humidity": 70}
        - {"is_door_open": false}
        - {"motor_speed": 2000}
        - {"water_flow": 100}
        - {"water_quality": 5}
        - {"water_level": 7}
        - {"rotating": 200}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301018/model-01/sn-001
    - payload
        - {"temperature": 28}
        - {"humidity": 40}
        - {"vibration": 300}
        - {"balance": 1}
        - {"current": 120}
        - {"lid_detection": "open"}



