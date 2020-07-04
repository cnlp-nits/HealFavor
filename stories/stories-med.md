## greet_reply
* greet_0_1
  - utter_welcome_0_1
  - utter_ask_booking_or_question_0_2



## appointment_only
* greet_0_1
  - utter_welcome_0_1
  - utter_ask_booking_or_question_0_2
* select_booking_0_2
  - utter_ask_doctor_speciality_0_3
* get_speciality_0_3{"speciality":"radiologist"}
  - slot{"speciality": "radiologist"}
  - utter_ask_doctor_name_0_4
* get_doctor_name_0_4{"doctor_name":"Gupta"}
  - utter_ask_date_and_month_0_5
* get_date_and_month_0_5{"date":"24","month":"jan"}
  - slot{"date": "24"}
  - slot{"month": "jan"}
  - utter_ask_time_0_6
* get_time_0_6{"time":"10:00"}
  - utter_final_booking_0_7
  - utter_any_other_question_0_8
* get_no_0_7
  - utter_have_a_good_day_0_9


## fever
* problem_fever_1_8
  - utter_ask_report_0_16
* have_report
  - utter_upload_0_17
  - utter_ask_headache_1_9
* problem_headache_1_9_2
  - utter_ask_nasal_1_5_1
* problem_not_nasal_1_5_2
  - utter_ask_duration_0_14
* long_duration_0_13
  - utter_hospital_0_15