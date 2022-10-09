

# Dima Usov


## Junior Frontend Developer


## Contact Information

**Email**: dmitry.usov@yahoo.com

**Telegram**: [@DUsov](t.me/DUsov)
___

## Summary
As an analyst in the retail industry, I often use programming to extract, transform, and load data. At some point, I become passionate about coding.  

So I intend to shift my career to software engineer with a focus on web development. More specifically, create applications using the Angular framework.  

To achieve my goal, I start taking Javascript/Front-end Mentoring Program at RS School (as of October 2022).


## Code example
Query which counts trip between 2019/01/01 and 2019/03/31 for dispatching_base_num B00987, B02060, B02279  

    -- Creating a partition and cluster table
    CREATE OR REPLACE TABLE
      de-zoomcamp-339014.trips_data_all.fhv_q4
    PARTITION BY
      DATE(pickup_datetime)
    CLUSTER BY
      dispatching_base_num AS
    SELECT
      * 
    FROM 
      `de-zoomcamp-339014.trips_data_all.fhv_tripdata_ext`;  

    -- Query
    SELECT
      COUNT(*) AS Total
    FROM
      `de-zoomcamp-339014.trips_data_all.fhv_q4`
    WHERE
     DATE(pickup_datetime) BETWEEN "2019-01-01" AND "2019-03-31"
     AND dispatching_base_num IN ('B00987', 'B02060', 'B02279');


## Courses
- M121: The MongoDB Aggregation Framework by [MongoDB University](https://university.mongodb.com/course_completion/8bbc243d-9a16-4d2d-9734-01db358cf39a?utm_source=copy&utm_medium=social&utm_campaign=university_social_sharing)
- From Data to Insights with Google Cloud by [Google Cloud on Coursera](https://coursera.org/share/67363dce1ab7f1db9a04c731e45bae19)
- Agile with Atlasian Jira [on Coursera](https://coursera.org/share/846435dab1929adb6376cdbc050f778f)  
- Applied Data Science with Python by [University of Michigan on Coursera](https://coursera.org/share/6453309e937fa96ca958f5a148633c51)


## Languages
- English - C1 ADVANCED according to [www.efset.org](https://www.efset.org/quick-check/)
- Russian - native