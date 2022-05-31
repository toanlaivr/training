## 1. Mục tiêu
- Nắm được tầm quan trọng của Unit test
- Nắm được phương pháp và kỹ thuật phân tích khi viết Unit Test
- Có thể viết test rspec được ở Controller và Model
## 2. Thời gian thực hiện
3 ngày (Tối đa 5 ngày nếu đi part time)
## 3. Cách thức thực hiện
- Áp dụng kiến thức học và tìm hiểu được để viết rspec tối thiểu cho 1 model và 1 controller viết đầy đủ unit test để đạt coverage là 100% 

- Từ thời điểm này đến hết Project 2 các pull request đều phải viết unit test nếu có sự thay đổi controller và model
- Coverage của model và controller cho đến lúc demo project 2 cần đạt >= 50%
## 4. Cài gem đo coverage
```
gem "simplecov-rcov"
gem "simplecov"
```

thêm vào spec_helper.rb
```
require "simplecov"
require "simplecov-rcov"
class SimpleCov::Formatter::MergedFormatter
  def format(result)
     SimpleCov::Formatter::HTMLFormatter.new.format(result)
     SimpleCov::Formatter::RcovFormatter.new.format(result)
  end
end
SimpleCov.formatter = SimpleCov::Formatter::MergedFormatter

SimpleCov.start "rails"
```

## 4. Link tài liệu
### 1. Homepage
http://rspec.info/<br>
[Github](https://github.com/rspec/rspec)

### 2. Document
[Slide]:
Rspec:
https://drive.google.com/drive/folders/1pmGs9YK6ScWkM0jXTapcwGGdnSdbQrd1

[Book]: 
https://drive.google.com/drive/folders/1_v-mZJjWj-RFDr_nEl5Mq6nqGsjoeu84

[References]
https://github.com/awesome-academy/Practice_Rspec
<br>
https://relishapp.com/rspec
<br>
http://www.relishapp.com/rspec/rspec-expectations/v/3-2/docs/built-in-matchers/type-matchers
<br>

### 3. Test style guide
[Vietnamese version](https://github.com/framgia/coding-standards/blob/master/vn/rails/test.md)

[English version](https://github.com/framgia/coding-standards/blob/master/eng/rails/test.md)

### 4. Some Gems
https://github.com/thoughtbot/shoulda-matchers
