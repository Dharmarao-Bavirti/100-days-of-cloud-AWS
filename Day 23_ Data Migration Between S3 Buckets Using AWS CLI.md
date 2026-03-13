# Day 23: Data Migration Between S3 Buckets Using AWS CLI

- **Create a New Private S3 Bucket**: Name the bucket `nautilus-sync-3975`.

- **Data Migration**: Migrate the entire data from the existing `nautilus-s3-1332` bucket to the new `nautilus-sync-3975` bucket.

- **Ensure Data Consistency**: Ensure that both buckets have the same data.

- **Use AWS CLI**: Use the AWS CLI to perform the creation and data migration tasks.


1. Check existing `S3` buckets.

   ```bash
   aws s3 ls
   ```

2. Create a private S3 bucket `nautilus-sync-3975`

   ```bash
   aws s3api create-bucket \
    --bucket nautilus-sync-3975 \
    --region us-east-1
    ```

3. Migrate data from old bucket to new bucket

   ```bash
   aws s3 sync s3://nautilus-s3-1332 s3://nautilus-sync-3975
   ```

4. Ensure data consistency

   ```bash
   aws s3 ls s3://nautilus-s3-1332 --recursive | wc -l
   aws s3 ls s3://nautilus-sync-3975 --recursive | wc -l
   ```
      
