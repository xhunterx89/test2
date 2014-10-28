Collider không tự nhiên có, đối với những đối tượng cơ bản như Cube, Plant, Sphere, Cylinder… là những đối tượng built-in của Unity, khi tạo ra, chúng được Unity gán sẵn các Collider tương ứng, nhưng đối với một mô hình được nhập (Import) từ bên ngoài, chúng ta phải tự gán cho chúng thông qua các lựa chọn ở menu: Component -> Physics. Tùy vào hình dáng, kích thước và vai trò của Object trong game mà chúng ta có những lựa chọn hay kết hợp các lựa chọn sao cho phù hợp. Và không phải đối tượng nào cũng buộc phải có Collider, như đã đề cập thì Colldier liên quan đến va chạm, liên quan đến vật lí, đây là những thành phần sẽ ảnh hương rất nhiều đến FPS của game, cụ thể là càng có nhiều Collider thì game sẽ càng nặng, nên chúng ta phải lưu ý chỉ nên attach Collider vào những đối tượng mà chúng ta muốn chúng có thể tương tác, đồng thời nên hạn chế sử dụng Mesh Collider – loại Collider dễ gây nặng game nhất.

Chúng ta có thể lưu ý những thông số cơ bản sau:

- Mass: Khối lượng

- Drag và Angular Drag: Độ ma sát khi di chuyển và khi xoay

- Use gravity (boolean): Vật có chịu tác động của trọng lực không? Hãy thử bỏ check giá trị này, chúng ta sẽ thấy đối tượng Cube không rơi, cho dù chúng ta có cho khối lượng nó lớn đến mức nào cũng thế.

Rigidbody còn là một Class trong Unity API, Class này sẽ cung cấp cho chúng ta chủ yếu các Function về lực, vận tốc, gia tốc để chúng ta xử lí các vấn đề về vận tốc, va chạm, các vụ nổ, … trong game.

-Tiếp theo chúng ta sẽ tìm hiểu về Physic Meterials

Unity mang đến cho chúng ta một khái niệm là “Physic material – vật liệu vật lý” cho phép chúng ta quy định Object được làm từ chất liệu gì, ví dụ như cao su, gỗ, kim loại, … Physic material gắn liền với Collider hay cụ thể nó là một giá trị của Component Collider. Mặc định Unity cung cấp chúng ta một vài built-in Physic material, tuy nhiên chúng ta hoàn toàn có thể tạo thêm bất kỳ cái nào mà chúng ta muốn thông qua hỗ trợ của Unity. Ở đây tôi sẽ không đề cập làm thế nào để tạo ra Physic material, mà chỉ muốn chúng ta lưu ý đến tác dụng của chúng, khi gán Physic material vào Object, các hiện tượng vật lý diễn ra với đối tượng sẽ tuân theo vật liệu đó, ví dụ như khi gán Bouncy cho Cube, khi rơi và va chạm với Floor, Cube sẽ tâng lên như một quả bóng.

Lưu ý: Để Import Physic material vào dự án làm như sau: Click phải ở cửa sổ Project -> Import Package -> Physic material hoặc chọn tương tự ở menu Asset.
Sau khi import xong thì bạn chọn Cube, bên tab Inspector tại Box Collider->Material bạn chọn Bouncy, sau đó Play xem có kết quả.

Tham khảo: http://www.unity3d.com.vn/
