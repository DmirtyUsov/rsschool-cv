# Mickey Mouse


## Junior Frontend Developer


## Contact Information

**Email**: MickeyMouse@DisneyWorld.com

___

## Summary
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam suscipit pharetra velit non finibus. Nulla tempor eros finibus semper dignissim. Donec posuere libero sed massa accumsan, eget facilisis orci tincidunt. Curabitur fringilla ipsum eu tellus sodales, vel ultrices augue congue. Suspendisse vulputate fermentum diam eget lacinia. Pellentesque elementum, massa a pharetra vehicula, lacus augue semper erat, eu suscipit urna ante eu quam. Nunc semper ante ac mi dapibus porttitor.

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


## Education
Disney University, Los Angeles, CA  
Bachelor of Arts in Happiness, Bringing Joy and Diplomacy, May, 2000 GPA: 3.5

## Languages
Fluent in all languages 