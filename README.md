# 実行されたSQL
## 先に実行されたメソッド（testGetClaimListByCriteria2）
```sql
2020-08-05 04:57:47.501  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : テストNo.2
2020-08-05 04:57:47.679 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        claim0_.id as id1_0_,
        claim0_.accident_date as accident2_0_,
        claim0_.base_in_charge as base_in_3_0_,
        claim0_.claim_number as claim_nu4_0_,
        claim0_.contractor_name as contract5_0_,
        claim0_.department_in_charge as departme6_0_,
        claim0_.insurance_type as insuranc7_0_,
        claim0_.insured_name as insured_8_0_,
        claim0_.update_date as update_d9_0_ 
    from
        claim claim0_ 
    where
        claim0_.claim_number=?
2020-08-05 04:57:47.684 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [VARCHAR] - [12345678910]
2020-08-05 04:57:47.717 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.claim_id as claim_id4_2_0_,
        fraudscore0_.id as id1_2_0_,
        fraudscore0_.id as id1_2_1_,
        fraudscore0_.claim_id as claim_id4_2_1_,
        fraudscore0_.claim_category as claim_ca2_2_1_,
        fraudscore0_.scoring_date as scoring_3_2_1_ 
    from
        fraud_score_history fraudscore0_ 
    where
        fraudscore0_.claim_id=?
2020-08-05 04:57:47.718 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.734 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.735 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [2]
2020-08-05 04:57:47.737 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.737 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [4]
2020-08-05 04:57:47.740 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.740 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [3]
2020-08-05 04:57:47.742 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.742 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.743 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.744 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [2]
2020-08-05 04:57:47.745 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.746 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.771  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : claimList:[Claim(Id=1, claimNumber=12345678910, insuredName=鈴木一郎, contractorName=山田次郎, departmentInCharge=第一部署, baseInCharge=東京本社, insuranceType=スポ協, updateDate=2020-07-25T12:00:00.000Z, accidentDate=2020-07-25T12:00:00.000Z)]
2020-08-05 04:57:47.772  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : claimList.size():1
```

## 後に実行されたメソッド（testGetClaimListByCriteria2）
```sql
2020-08-05 04:57:47.808  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : テストNo.1
2020-08-05 04:57:47.809 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        claim0_.id as id1_0_,
        claim0_.accident_date as accident2_0_,
        claim0_.base_in_charge as base_in_3_0_,
        claim0_.claim_number as claim_nu4_0_,
        claim0_.contractor_name as contract5_0_,
        claim0_.department_in_charge as departme6_0_,
        claim0_.insurance_type as insuranc7_0_,
        claim0_.insured_name as insured_8_0_,
        claim0_.update_date as update_d9_0_ 
    from
        claim claim0_ 
    where
        claim0_.claim_number=?
2020-08-05 04:57:47.810 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [VARCHAR] - [12345678910]
2020-08-05 04:57:47.811 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.claim_id as claim_id4_2_0_,
        fraudscore0_.id as id1_2_0_,
        fraudscore0_.id as id1_2_1_,
        fraudscore0_.claim_id as claim_id4_2_1_,
        fraudscore0_.claim_category as claim_ca2_2_1_,
        fraudscore0_.scoring_date as scoring_3_2_1_ 
    from
        fraud_score_history fraudscore0_ 
    where
        fraudscore0_.claim_id=?
2020-08-05 04:57:47.812 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [2]
2020-08-05 04:57:47.812 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.claim_id as claim_id4_2_0_,
        fraudscore0_.id as id1_2_0_,
        fraudscore0_.id as id1_2_1_,
        fraudscore0_.claim_id as claim_id4_2_1_,
        fraudscore0_.claim_category as claim_ca2_2_1_,
        fraudscore0_.scoring_date as scoring_3_2_1_ 
    from
        fraud_score_history fraudscore0_ 
    where
        fraudscore0_.claim_id=?
2020-08-05 04:57:47.813 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.814 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.816 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [4]
2020-08-05 04:57:47.817 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.817 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [3]
2020-08-05 04:57:47.818 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.818 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [2]
2020-08-05 04:57:47.820 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.820 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [8]
2020-08-05 04:57:47.821 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.821 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [7]
2020-08-05 04:57:47.822 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.823 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [4]
2020-08-05 04:57:47.826 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.827 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [3]
2020-08-05 04:57:47.830 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_0_,
        fraudscore0_.id as id1_1_0_,
        fraudscore0_.id as id1_1_1_,
        fraudscore0_.fraud_score_history_id as fraud_sc5_1_1_,
        fraudscore0_.model_category_name as model_ca2_1_1_,
        fraudscore0_.rank as rank3_1_1_,
        fraudscore0_.score as score4_1_1_ 
    from
        fraud_score_details fraudscore0_ 
    where
        fraudscore0_.fraud_score_history_id=?
2020-08-05 04:57:47.830 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.832 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.832 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [6]
2020-08-05 04:57:47.833 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.833 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [5]
2020-08-05 04:57:47.834 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.834 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [2]
2020-08-05 04:57:47.836 DEBUG 61548 --- [           main] org.hibernate.SQL                        : 
    select
        reasons0_.fraud_score_detail_id as fraud_sc6_3_0_,
        reasons0_.id as id1_3_0_,
        reasons0_.id as id1_3_1_,
        reasons0_.description as descript2_3_1_,
        reasons0_.feature_description as feature_3_3_1_,
        reasons0_.fraud_score_detail_id as fraud_sc6_3_1_,
        reasons0_.rank as rank4_3_1_,
        reasons0_.score as score5_3_1_ 
    from
        reasons reasons0_ 
    where
        reasons0_.fraud_score_detail_id=?
2020-08-05 04:57:47.837 TRACE 61548 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
2020-08-05 04:57:47.850  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : claimList:[Claim(Id=1, claimNumber=12345678910, insuredName=鈴木一郎, contractorName=山田次郎, departmentInCharge=第一部署, baseInCharge=東京本社, insuranceType=スポ協, updateDate=2020-07-25T12:00:00.000Z, accidentDate=2020-07-25T12:00:00.000Z), Claim(Id=2, claimNumber=12345678910, insuredName=鈴木一郎, contractorName=山田次郎, departmentInCharge=第一部署, baseInCharge=東京本社, insuranceType=スポ協, updateDate=2020-07-25T12:00:00.000Z, accidentDate=2020-07-25T12:00:00.000Z)]
2020-08-05 04:57:47.850  INFO 61548 --- [           main] com.example.service.ClaimServiceTest     : claimList.size():2
```
