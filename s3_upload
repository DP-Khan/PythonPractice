import boto3
import argparse
parser = argparse.ArgumentParser()
parser.add_argument("Access_Key", type=str)
parser.add_argument("Access_Key_ID", type=str)
args = parser.parse_args()

client = boto3.client(
    's3',
    aws_access_key_id=args.Access_Key,
    aws_secret_access_key=args.Access_Key_ID,
)

response = client.list_objects(
    Bucket="tst-bucket-jenkins"
)

print(response)
