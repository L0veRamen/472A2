# COMP472 Assignment A2
## Team: RoboCops
### Team Members:
- Rongxi Meng (40045067)
- Chen Qian (27867808)


# Load your CSV file into a pandas DataFrame
df = pd.read_csv('./datasets/synonym.csv')

# load model
word2vec_model = api.load("word2vec-google-news-300")

# Save the DataFrame with the predicted synonyms and labels to a CSV file
output_file_path = './output/task_1/word2vec-google-news-300-details.csv'

# Save the analysis DataFrame to a CSV file
df_task_1_analysis.to_csv('./output/task_1/analysis.csv', index=False, header=False)

# Convert the results to a DataFrame and save to CSV
df_task_2_analysis = pd.DataFrame(results)
df_task_2_analysis.to_csv('./output/task_2/analysis.csv', index=False, header=False)

# Directory containing your book files
book_directory = './books/' 
