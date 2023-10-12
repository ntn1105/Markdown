## Git là gì?

- **Git** là một hệ thống quản lí phiên bản phân tán (Distributed Version Control System – DVCS) mã nguồn mở và miễn phí được sử dụng để quản lý hiệu quả các dự án từ nhỏ đến rất lớn. Git được ra đời vào năm 2005 do Linus Torvalds tạo ra.

- **Git** cung cấp cho mỗi lập trình viên một kho lưu trữ riêng chứa toàn bộ lịch sử thay đổi code. Nó thường được sử dụng trong phát triển phần mềm để quản lý mã nguồn. Các kho lưu trữ Git được kết nối cục bộ, cho phép các lập trình viên làm việc trên máy của riêng họ, nhưng cũng được kết nối với một kho lưu trữ dùng chung.

## Đặc điểm của git?

**_Về cách xử lý dữ liệu_**

Git coi dữ liệu của nó là một tập các ảnh (snapshot) của hệ thống tập tin. Điều này có nghĩa là mỗi phiên bản của dự án (có thể hiểu là một commit) sẽ là tập hợp của một số ảnh lưu lại nội dung của các tập tin của phiên bản đó. Điều này mang đến nhiều tiện lợi cho việc theo dõi lịch sử, phục hồi dữ liệu và phân nhánh.

**_Thao tác với dữ liệu_**

Hầu hết các thao tác với dữ liệu của Git có thể thực hiện cục bộ. Git thực hiện được việc này vì toàn bộ dữ liệu của dự án đều được lấy về và lưu trữ trên máy tính của người dùng.
Với tính năng này của Git, người dùng có thể làm việc trong nhiều trường hợp mà không nhất thiết phải có kết nối Internet. Điều này mang đến nhiều lợi thế cho Git so với các hệ thống quản lý dữ liệu khác.

**_Tính toàn vẹn_**

Các thay đổi trong Git được tham chiếu bằng một mã sử dụng cơ chế mã hóa SHA-1. Đồng thời, các thay đổi trong Git đều được thêm vào cơ sở dữ liệu do đó rất khó bị mất khi thay đổi và truyền tải dữ liệu. Với Git, người dùng có thể thoải mái thử nghiệm, lưu trữ mà không sợ ảnh hưởng đến dự án.

## Tại sao phải sử dụng git?

- Git dễ sử dụng, an toàn và nhanh chóng.
- Có thể giúp quy trình làm việc code theo nhóm đơn giản hơn rất nhiều bằng việc kết hợp các phân nhánh (branch).
- Bạn có thể làm việc ở bất cứ đâu vì chỉ cần clone mã nguồn từ kho chứa hoặc clone một phiên bản thay đổi nào đó từ kho chứa, hoặc một nhánh nào đó từ kho chứa.
- Dễ dàng trong việc deployment sản phẩm.

## Cách cài đặt git?

Bạn có thể cài đặt Git bằng cách tải trực tiếp từ trang web chính thức của Git
**_[Download Git](https://git-scm.com/downloads)_**

## Github là gì?

**GitHub** là một hệ thống quản lý dự án và phiên bản code, hoạt động giống như một mạng xã hội cho lập trình viên. Các lập trình viên có thể clone lại mã nguồn từ một repository và Github chính là một dịch vụ máy chủ repository công cộng, mỗi người có thể tạo tài khoản trên đó để tạo ra các kho chứa của riêng mình để có thể làm việc.

## Repository là gì ? Cách tạo ra 1 Repository

**Repository** được hiểu là một kho lưu trữ nơi chứa các files của dự án. Các file đấy có thể là code, hình ảnh, âm thanh hoặc tất cả mọi thứ liên quan đến dự án. Bạn sẽ tổ chức kho lưu trữ của mình dưới nhiều hình thức không giống nhau, hai loại kho lưu giữ trong Github là Local Repository và Remote Repository.

### Cách tạo ra 1 Repository

**Bước 1:** Vào Github tại đây, sau đó đăng ký một tài khoản bằng việc click vào **"Sign up for Github"**.
Sau khi hoàn tất dăng nhập.Nhấn nút **"New repository"**

**Bước 2:** Nhập tên Repository và nhấn nút **“Create Repository”**. Ngoài những điều ấy ra, bạn cũng có thể thêm mô tả cho Repository (lựa chọn này không bắt buộc).

Trong đó, bạn cần lưu ý:

- Repository mặc định là công khai. Nếu dự án của bạn chỉ ước muốn quản lý nội bộ thì chọn **"Private"**.
- Bạn có thêm một **"README file"** để giới thiệu Repository kèm với một tệp .gitignore. Github đã cho bạn sẵn template .gitignore, nên bạn chỉ phải chọn một template phù hợp với mã nguồn dự án là được.

## Phân biệt local branch và remote branch?

**_Local Repository:_** là một loại repository nằm trên máy tính của bạn, repository này có nhiêm vụ đồng bộ hóa với remote repository bằng các lệnh của git.

**_Remote Repository:_** là một loại repository được cài đặt trên server chuyên dụng. Ví dụ như: GitHub, GitLab, Bitbucket,…

## Git clone, push, pull, fetch, merge, add, commit?

- **Git Clone:** Lệnh này được sử dụng để sao chép một kho lưu trữ (repository) từ một kho chứa từ xa (remote repository) vào máy tính của bạn
- **Git Push:** Lệnh này được sử dụng để đẩy (push) các thay đổi từ máy tính của bạn lên kho chứa từ xa.

- **Git Pull:** Lệnh này được sử dụng để cập nhật mã nguồn từ kho chứa từ xa và tự động thực hiện một quá trình Merge (hợp nhất) để hợp nhất các thay đổi từ kho chứa từ xa vào nhánh hiện tại trên máy tính của bạn.

- **Git Fetch:** Lệnh này được sử dụng để tải thông tin từ kho chứa từ xa mà không hợp nhất (merge) các thay đổi vào mã nguồn của bạn.

- **Git Merge:** Lệnh này được sử dụng để hợp nhất các nhánh khác nhau lại với nhau. Thường được sử dụng sau khi bạn đã có các thay đổi từ một nhánh khác (thông qua Git Pull hoặc thao tác khác).

- **Git Add:** Lệnh này được sử dụng để đánh dấu (staging) các tệp tin hoặc thư mục đã thay đổi để chuẩn bị cho việc commit.

- **Git Commit:** Lệnh này được sử dụng để lưu trạng thái hiện tại của các tệp đã được đánh dấu (staged) trong một lịch sử phiên bản.

## Các trạng thái của files trong git là gì?

**1.** Trạng thái đã theo dõi (Tracked): Đây là trạng thái của các tệp đã được Git theo dõi và được quản lý trong kho lưu trữ của bạn. Các tệp trong trạng thái đã theo dõi có thể ở trong một trong hai trạng thái sau:

- Trạng thái đã sửa đổi (Modified): Đây là trạng thái của các tệp đã được sửa đổi so với phiên bản cuối cùng trong kho lưu trữ. Các thay đổi này chưa được đánh dấu là đã chuẩn bị commit.

- Trạng thái đã đánh dấu (Staged): Các tệp trong trạng thái này đã được thêm vào vùng chuẩn bị (staging area) để chuẩn bị cho việc commit. Điều này có nghĩa rằng Git biết rằng bạn muốn lưu lại trạng thái hiện tại của các tệp này trong phiên bản tiếp theo.

**2.** Trạng thái chưa theo dõi (Untracked): Đây là trạng thái của các tệp mà Git chưa theo dõi. Các tệp này không nằm trong lịch sử phiên bản của Git và không được quản lý.

## Conflict trong git là gì? Tại sao lại xảy ra conflict? Cách giải quyết như thế nào?

**Conflict trong git là gì?**

**Git conflict** là sự kiện xảy ra khi Git không thể tự động giải quyết sự khác biệt về code giữa hai lần commit. Git chỉ có thể merge các thay đổi một cách tự động nếu các lần commit nằm trên các dòng hoặc branch khác nhau.

**Tại sao lại xảy ra conflict?**

- Sửa đổi đồng thời

- Sự phân nhánh và ghép nối (branching and merging)

- Sửa đổi xung đột trong cùng một dòng mã

- Ghép nối không tự động (automatic merging fails)

- Xung đột về tên tệp hoặc thư mục

**Cách giải quyết như thế nào?**

**1,Xác định xung đột:** Sử dụng lệnh git status để xác định các tệp bị xung đột trong kho lưu trữ của bạn. Git sẽ liệt kê các tệp mà cần phải giải quyết xung đột.

**2,Mở tệp xung đột:** Sử dụng trình soạn thảo để mở các tệp bị xung đột. Trong tệp, bạn sẽ thấy các ký tự đánh dấu xung đột, chẳng hạn như <<<<<<<, =======, và >>>>>>>, để chỉ ra các phần bị xung đột giữa hai phiên bản của mã nguồn.

**3,Giải quyết xung đột thủ công:** Sửa các phần bị xung đột bằng cách chọn phiên bản nào cần giữ lại hoặc kết hợp chúng lại một cách thủ công. Sau khi bạn đã hoàn thành, xóa các đánh dấu xung đột và lưu tệp.

**4,** Sau khi bạn đã giải quyết xung đột thủ công, sử dụng lệnh git add để đánh dấu các tệp đã giải quyết xung đột cho việc theo dõi

**5,Commit thay đổi đã giải quyết xung đột:** Sau khi bạn đã giải quyết xung đột cho tất cả các tệp cần thiết, sử dụng lệnh git commit để tạo một commit mới chứa các thay đổi đã giải quyết xung đột.

**6,Tiếp tục quá trình ghép nối hoặc gửi thay đổi lên kho lưu trữ từ xa (remote):** Nếu bạn đang làm việc trên một nhánh riêng của bạn và muốn ghép nối thay đổi với nhánh chính (hoặc nhánh từ xa), sử dụng lệnh git merge hoặc git pull. Nếu bạn làm việc trên một nhánh từ xa và muốn gửi thay đổi lên kho lưu trữ từ xa, sử dụng lệnh git push.
