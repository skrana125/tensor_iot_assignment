# tensor_iot_assignment
1. I have created through replit and the main code file is main.py rest is driver code/file which is added in the repository
2. I have commented the the way to load the file in the aws s3 that the code that I wrote in the main.py
     def upload_to_s3(self, file_name, bucket_name):
       s3 = boto3.client("s3")
       s3.upload_file(file_name, bucket_name, file_name)
   
4. this is the way to load the file into the s3
   #Example usage
   parking_lot.upload_to_s3("mapping.json", "my-s3-bucket")

5. Output throught this file will be like
   Example 1
  Car with license plate ABC1234 parked successfully in spot 16
  Car with license plate DEF4567 was not able to park in spot 16
  Car with license plate DEF4567 parked successfully in spot 7
  Car with license plate GHI7890 parked successfully in spot 0

  example 2:
  Car with license plate ABC1234 parked successfully in spot 17
  Car with license plate DEF4567 parked successfully in spot 2
  Car with license plate GHI7890 parked successfully in spot 19

  #Used IDE replit an online ide
