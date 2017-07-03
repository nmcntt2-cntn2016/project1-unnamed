<h2 align="center"> <a href="http://nmcntt2-cntn2016.github.io/unnamed"> -- WEBSITE -- </a></h2>
<h2 align="center"> <a href="http://nmcntt2-cntn2016.github.io/unnamed/demo.html"> -- DEMO --  </a></h2>
<h2 align="center">TEAM UNNAMED</h1>

<table>
	<tr>
		<th>ID</th>
	    <th>Name</th> 
	  </tr>
	  <tr>
	    <td>1612377</td>
	    <td>Tô Hiếu Minh</td>
	  </tr>
	  <tr>
	    <td>1612418</td>
	    <td>Phạm Lưu Trọng Nghĩa</td>
	  </tr>
	  <tr>
	    <td>1612521</td>
	    <td>Trang Trung Hoàng Phúc</td>
	  </tr>
		 <tr>
	    <td>1612703</td>
	    <td>Nguyễn Thị Tình</td>
	  </tr>
	</table>
	
## SwiftCHEM - Trang web mô tả thí nghiệm hóa học
<p align="center"><img src="http://i.imgur.com/aFbfcOb.jpg"></p> 

 
## Thực trạng :
* Thực trạng, một số trường ở Việt Nam không có đủ cơ sở vật chất cho học sinh làm thí nghiệm.
* Gần đây xảy ra nhiều vụ nổ hóa chất gây thiệt hại về tài sản và tính mạng con người.
* Ở Việt Nam chưa có nhiều giải pháp để giải quyết các vấn đề này.
* Một số app và trang web (ChemLab, phET interactive simulations...) có các tính năng thí nghiệm nhưng khó sử dụng, không trực quan và sử dụng nhiều thuật ngữ chuyên ngành.

## Mục đích :
* Giúp học sinh, sinh viên tiết kiệm thời gian và tăng sự hứng thú khi học hóa, học tập tốt hơn.
* Giúp học sinh, sinh viên tiếp cận, làm quen với thực hành thí nghiệm hoá học, tránh lý thuyết suông.
* Giúp tiết kiệm chi phí xây dựng phòng thí nghiệm, mua các chất hóa học; giảm tai nạn đáng tiếc.

## Tính năng :
* Cung cấp công cụ học tập có các chức năng:
	* Mô tả hiện tượng một cách trực quan bằng ảnh động / video.
	* Tự động cân bằng và hiển thị thông tin các chất liên quan.
	* Điều chế chất mới từ chất ban đầu.
	* Cung cấp diễn đàn trực tuyến giúp người học có thể trao đổi được với nhau
	* Phân biệt các chất được nhập vào ( nếu được ).
	
## Cách thực hiện :
* Công nghệ (nếu là web): Các công cụ, thư viện nhóm sẽ sử dụng để làm nền tảng web SwiftCHEM:
	* Front-end:
		* Ngôn ngữ: html/css.
		* Framework: Angular.
		* Library: jQuery AJAX methods, bootstrap, angular material design.
	* Back-end:
		* Ngôn ngữ: Javascript.
		* Platform: Node.js.
		* ORM (Object Relational Mapping): Bookshelf.
		* SQL builder: Knex.
	* Database: MySQL.
* Các thuật toán, cấu trúc dữ liệu sẽ áp dụng:
	* Cân bằng phương trình: Sử dụng thuật Gauss-Jordan để giải hệ phương trình tuyến tính tìm ra hệ số cho các chất . Sau đó tìm hệ số thích hợp nhân lên để khử mẫu số cho bộ nghiệm.
	<p align="center"><img src="https://media.giphy.com/media/3o7btVyBxOHteapl7y/giphy.gif"></p>
	
	* Điều chế các chất : Liên kết các phương trình với nhau để tạo ra chuỗi phản ứng điều chế với thuật Depth First Search, ta sẽ tìm với độ sau tối đa là 3. Tức có nghĩa để điều chế từ chất A qua B, ta sẽ sử dụng tối đa 3 phản ứng thôi.
		* Ta có thể điều chế một dãy các chất (input nhập vào nhiều hơn 2).
		* Tối ưu bằng cách xem người dùng hay tìm kiếm điều chế chất nào và giữ cố định kết quả đó lại để sử dụng cho sau này.
		
* Do các chất hóa học thường có một số dạng như loại dung dịch, rắn, hơi, ... và chỉ khác nhau về màu sắc, hiện tượng nên việc tạo các ảnh động mô tả hiện tượng hóa học có thể hoàn thành nhanh chóng bằng tool team sẽ tự làm đối với các phản ứng mang tính tương đồng ví dụ như BaSO4 + CuCl2 và NaSO4 + CuCl2. Ngoài ra đối với các phản ứng có đặc trưng riêng thì sẽ được làm riêng.


 
## Cách thức hoạt động và phát triển:
* Đăng dự án lên Kickstarter để tìm nguồn kinh phí thuê người nhập liệu. Dự đoán dự án sẽ được đưa vào hoạt động sau 3 tháng. Nếu không kiếm đủ tiền để thuê người thì nhóm sẽ tự làm các công việc đó, dự đoán sẽ đưa vào hoạt động sau 8 tháng.
* Sau khi đã hoạt động thì có thêm tính năng để người dùng có thể đóng góp các phản ứng và các hình ảnh thí nghiệm. Sẽ có một đội ngũ chuyên kiểm duyệt nội dung do người dùng đóng góp.
* Tạo một tài khoản ngân hàng để người sử dụng có thể donate được giúp trang web có thể tiếp tục được hoạt động.
* Trang web sẽ hoàn toàn miễn phí và nhắm đến đối tượng người dùng là học sinh (80%) và giáo viên (20%), chủ yếu ở Việt Nam.

## Các môn học cần thiết để thực hiện dự án
* Lập trình Web
* Hệ quản trị cơ sở dữ liệu
* An toàn và bảo mật trong hệ thống thông tin
* Cấu trúc dữ liệu và giải thuật
* Tư duy thuật toán
* Quản lí dự án
* Nếu mở rộng ra app cho các thiết bị như PC, phone thì cần:
	* Lập trình Windows
	* Thiết kế giao diện
	* Công nghệ XML và ứng dụng

## POSTER
<p align="center"><img src="http://i.imgur.com/LLhycN0.jpg"></p>
