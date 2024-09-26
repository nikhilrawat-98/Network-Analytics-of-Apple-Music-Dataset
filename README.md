# Network Analytics of Apple Music Dataset

This project involves performing network analytics on the **Apple Music Dataset**, utilizing various centrality measures, community detection techniques, and visualization tools to uncover meaningful patterns and insights into the network structure of music tracks and their connections. The project applies fundamental network analytics concepts to analyze the relationships between music tracks based on features like genres, artists, and popularity.

## Project Overview

- **Objective**: The primary goal of this project is to perform network analysis on the Apple Music dataset to identify key tracks and genres, detect communities within the network, and understand the influence of different music tracks using various centrality measures.
- **Key Methods**: Centrality measures (degree, closeness, betweenness), Community detection (Louvain, Girvan-Newman), and network visualization.
- **Tech Stack**: Python, NetworkX, Pandas, Matplotlib, Gephi for visualization.

## Dataset

The dataset consists of various Apple Music tracks with information on features such as genres, artists, popularity, and connections between tracks.

### Dataset Features:
- `Track ID`: Unique identifier for each track.
- `Artist`: The artist or band associated with the track.
- `Genre`: The genre of the track.
- `Popularity`: The popularity score of the track.
- `Connections`: The edges in the network, representing relationships between tracks based on shared features or genres.

## File Structure

- **`Code.ipynb`**: Jupyter notebook containing the code for the network analytics, including data processing, centrality calculations, community detection, and visualization.
- **`Report.pdf`**: Detailed report discussing the methodology, results, and key findings from the network analysis.
- **`apple_music_dataset.csv`**: Dataset containing the Apple Music data used for network analysis.
- **`requirements.txt`**: Python dependencies required to run the project.

## Methods and Results

The following methods were applied to the dataset:

### 1. Centrality Measures:
- **Degree Centrality**: Identifies tracks with the most connections to other tracks.
- **Betweenness Centrality**: Highlights tracks that act as bridges between different parts of the network.
- **Closeness Centrality**: Determines the proximity of a track to all others in the network.

### 2. Community Detection:
- **Louvain Method**: Used to detect communities of closely related tracks based on shared features like genre or artist.
- **Girvan-Newman Method**: Applied to identify communities by progressively removing edges with high betweenness centrality.

### 3. Visualization:
- Gephi was used to visualize the network structure, highlighting important nodes (tracks) and communities.

### Key Findings:
- **Highly Central Tracks**: Certain tracks stood out as highly connected, bridging different communities, especially in popular genres.
- **Communities**: Detected communities revealed clusters of tracks from similar genres, with clear boundaries between popular genres and niche ones.

## Usage

The Jupyter notebook demonstrates the following:
1. **Data Pre-processing**:
    - Loading the Apple Music dataset.
    - Building the network from the dataset, where nodes represent tracks and edges represent connections.
2. **Network Analysis**:
    - Calculating centrality measures for each track in the network.
    - Applying community detection algorithms to find clusters within the network.
3. **Visualization**:
    - Generating network visualizations using Matplotlib and exporting the data for Gephi.

## Installation

To run the project locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Network-Analytics-Apple-Music.git
    cd Network-Analytics-Apple-Music
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook:
    ```bash
    jupyter notebook
    ```

## Acknowledgements

This project was developed as part of the MSc in Business Analytics program at Bayes Business School.

## License

MIT License
