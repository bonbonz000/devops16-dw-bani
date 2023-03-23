Question :
1. Menggunakan 2 server, jalankan Load Balancing yang berfungsi dengan baik

Answer :

setup reverse proxy and the load balancing nginx (note the upstream must be same)
![ch 0](https://user-images.githubusercontent.com/91004163/227375785-a3fb9fef-439c-4ce1-9fbb-1d78dd31b23c.png)


2 server running same application over port 3000

![ch 1](https://user-images.githubusercontent.com/91004163/227375697-ee6ee187-2581-474d-8586-9f9a234d84c3.png)


one server is down, connection still running fine

![ch 2 serv down](https://user-images.githubusercontent.com/91004163/227375742-25b18d70-791b-4d6d-b297-59a76605c6a4.png)


