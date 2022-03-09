# Bookstore Customer Clustering (K-Means Clustering)

# **Summary**

**Introduction**: 

How to make recommendation models? I was always curious about this topic and finally had a chance to learn K-NN Clustering, one of the most commonly used models for customer clustering and recommendation. When I discovered a data for customer’s rating for books on Kaggle, I realized that this will be the perfect dataset for practicing clustering customers by using their rating data

**Datasets**:

The data contains customer information, book information and customers’ rating for each book.

Its shape is 1031175 rows × 19 columns.

**Language and libraries**: Python, Pandas, Sklearn

**ML Algorithm**: K-Means Clustering

**Evaluation Metric**: Silhouette score (17 showed the best score)

![ex_screenshot](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/08094168-e376-4409-85a7-1704e3ddd83d/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220309%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220309T183314Z&X-Amz-Expires=86400&X-Amz-Signature=b4ea33dc7a65672001fcadeae7ded90d753cf0902046f5a7dd79ad471c896e43&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

**Final Result**: Clustered customers into 17 clusters

![ex_screenshot](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/657a0587-c74e-4fa5-980b-c81628dce3be/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220309%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220309T183404Z&X-Amz-Expires=86400&X-Amz-Signature=dc38279972b8165a68ed088a12aa7217428b71f6aea1fdd036949dc7122b1d80&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

**Takeaways and future study topics**:

1. We clustered customers, and then what will happen?
    
    After clustering customers into 17 groups, we can assume that customers in the same group have similar tastes in books. Therefore, now we can find the best rating books or book categories for each group and use them to recommend proper books to our customers. 
    
    However, having a meeting with marketers will be helpful to add more insights for making list for recommending book lists.
    
2. Limit on computational resource
    
    I merged minor categories which have less than 2000 counts to ‘other’ due to a limit on my laptop's resources. However, merging these categories can be a reason that why the ‘No preference’ group’s count is the biggest and cause a decrease in the accuracy of the model if the clusters are used for recommending books in reality. Therefore, more effort to improve the processing speed of the model is required for future projects.
