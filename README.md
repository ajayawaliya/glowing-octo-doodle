# glowing-octo-doodle

# server.py
from http.server import SimpleHTTPRequestHandler, HTTPServer

PORT = 8080

httpd = HTTPServer(("127.0.0.1", PORT), SimpleHTTPRequestHandler)
print(f"Serving locally on http://127.0.0.1:{PORT}")
httpd.serve_forever()
