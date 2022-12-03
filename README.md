# Agenda Mahasiswa Ilmu Komputer
##

## Data Mahasiswa Ilmu Komputer
<details>
<summary> Klik untuk Ekspan </summary>

### Create Mahasiswa
<table>
<tr>
    <td> <b>URL</b> </td>
    <td> {{baseURL}}/api/v1/mahasiswa</td>
</tr>
<tr>
    <td> <b>Method</b> </td>
    <td> POST </td>
</tr>
<tr>
    <td> <b>Header</b> </td>
    <td> Authorization : Bearer Token  </td>
</tr>    
<tr>
<td> <b>Body</b> </td>
<td>

``` json
{
    "nama" : "Rusdi Abdul Gani",
    "alamat" : "Kab Bogor",
    "hoby" : "Musik"
}    
```
</td>
</tr>
<tr>
<td> <b>Respon Success</b> </td>
<td>

``` json
{
    "code" : 201,
    "message" : "Data mahasiswa berhasil diinput",
    "data" : {
        "nim" : 2001,
        "nama" : "Rusdi Abdul Gani",
        "alamat" : "Bogor",
        "hoby" : "Musik"
    } 
}    
```
<tr>
<td> <b>Respon Conflict</b> </td>
<td>

``` json
{
    "code" : 409,
    "message" : "Nama Mahasiswa telah digunakan",
    "data" : {
        "value" : "Rusdi Abdul Gani",
        "property" : "nama",
        "location" : "body"
    } 
}    
```

</td>
</tr>
</table>
</details>
