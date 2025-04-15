#include <stdio.h>

#define MAX 10

int graph[MAX][MAX];
int visited[MAX];
int n;

void DFS(int vertex) {
    visited[vertex] = 1;
    printf("Visited %d\n", vertex);

    for (int i = 0; i < n; i++) {
        if (graph[vertex][i] == 1 && !visited[i]) {
            DFS(i);
        }
    }
}

int main() {
    int edges, u, v;

    scanf("%d", &n);
    scanf("%d", &edges);

    for (int i = 0; i < edges; i++) {
        scanf("%d %d", &u, &v);
        graph[u][v] = 1;
        graph[v][u] = 1;
    }

    DFS(0);

    return 0;
}
