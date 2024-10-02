# Finance Bank Loan Report [PBI]
## Introduction
### 1. About
- In order to monitor and assess our bank's lending activities and performance, Bank Loan Report provide insights into key loan-related metrics and their changes over time. The report will help manager make data-driven decisions, track loan portfolio's health, and identify trends that can inform lending strategies
### 2. Reasons for Analysing Bank Loan Data
Banks analyse loan data for several critical reasons:
- **Risk Assessment**: One of the primary purposes of analysing loan data is to assess the risk associated with lending to a particular individual or business. Banks use data to evaluate the creditworthiness of borrowers, predict default probabilities, and determine interest rates and lending terms.
- **Decision-making**: Loan data analysis supports the decision-making process when evaluating loan applications. Banks use data-driven models and algorithms to make informed lending decisions, such as approving or denying loan requests.
- **Portfolio Management**: Banks manage portfolios of loans, including mortgages, personal loans, and business loans. Data analysis helps banks monitor the health of these portfolios, identify underperforming loans, and optimize loan terms and pricing.
- **Fraud Detection**: Banks use data analysis to detect fraudulent loan applications and activities. Unusual patterns, inconsistencies, or discrepancies in loan data can trigger fraud alerts.
- **Regulatory Compliance**: Banks are subject to regulatory requirements that mandate the collection and reporting of loan data. Compliance with regulations such as the Home Mortgage Disclosure Act (HMDA) and the Know Your Customer (KYC) regulations requires data analysis and reporting.
- **Customer Insights**: Analysing loan data provides insights into customer behaviour, preferences, and needs. Banks can use these insights to tailor loan products and marketing strategies to specific customer segments.
- **Profitability Analysis**: Banks assess the profitability of their loan portfolios by analysing data related to interest income, loan origination costs, default rates, and collection efforts.
- **Market Research**: Data analysis helps banks understand market trends, competitive landscape, and customer demand. This information guides product development and market expansion strategies.
- **Credit Risk Management**: Banks continuously monitor and manage credit risk associated with their loans. Data analysis helps in setting risk management strategies, provisioning for potential losses, and stress testing loan portfolios.
- **Customer Retention**: Banks use data analysis to identify opportunities for retaining existing customers, such as offering loan refinancing options or additional financial products
### 3. Dataset
- A dataset containing information about a bank's loans
- Fields in the dataset: <br/>
  - **Loan ID:** Loan ID is a unique identifier assigned to each loan application or loan account. It serves as a primary key for tracking and managing individual loans. <br/>
  - **Address State:** Address State indicates the borrower's location. It helps in assessing regional risk factors, compliance with state regulations, and estimating default probabilities. <br/>
  - **Employee Length:** Employee Length provides insights into the borrower's employment stability. Longer employment durations may indicate greater job security.<br/>
  - **Employee Title:** Employee Title specifies the borrower's occupation or job title. It helps lenders understand the source of the borrower's income.<br/>
  - **Grade:** Grade represents a risk classification assigned to the loan based on creditworthiness. Higher grades signify lower risk.<br/>
  - **Sub Grade:** Sub Grade refines the risk assessment within a grade, providing additional risk differentiation.<br/>
  - **Home Ownership:** Home Ownership indicates the borrower's housing status. It offers insights into financial stability.<br/>
  - **Issue Date:** Issue Date marks the loan's origination date. It's crucial for loan tracking and maturity calculations.<br/>
  - **Last Credit Pull Date:** Last Credit Pull Date records when the borrower's credit report was last accessed. It helps monitor creditworthiness.<br/>
  - **Last Payment Date:** Last Payment Date marks the most recent loan payment received. It tracks the borrower's payment history.<br/>
  - **Loan Status:** Loan Status indicates the current state of the loan (e.g., fully paid, current, default). It tracks loan performance.<br/>
  - **Next Payment Date:** Next Payment Date estimates the date of the next loan payment. It assists in cash flow forecasting.<br/>
  - **Purpose:** Purpose specifies the reason for the loan (e.g., debt consolidation, education). It helps understand borrower intentions.<br/>
  - **Term:** Term defines the duration of the loan in months. It sets the repayment period.<br/>
  - **Verification Status:** Verification Status indicates whether the borrower's financial information has been verified. It assesses data accuracy.<br/>
  - **Annual Income:** Annual Income reflects the borrower's total yearly earnings. It assesses repayment capacity.<br/>
  - **DTI (Debt-to-Income Ratio):** DTI measures the borrower's debt burden relative to income. It gauges the borrower's capacity to take on additional debt.<br/>
  - **Instalment:** Instalment is the fixed monthly payment amount for loan repayment, including principal and interest.<br/>
  - **Interest Rate:** Interest Rate represents the annual cost of borrowing expressed as a percentage. It determines the loan's cost.<br/>
  - **Loan Amount:** Loan Amount is the total borrowed sum. It defines the principal amount.<br/>
## Analysis & Visualization
1. Summary Page
![summary](https://github.com/user-attachments/assets/cd615676-80e7-4ac2-9592-d020238c2fd1) <br />
- Tổng hồ sơ vay (Total Loan Applications):
  - 38.6K đơn vay đã được xử lý.
  - Số lượng đơn vay tăng 6.9% so với tháng trước (MoM), điều này cho thấy nhu cầu vay vốn đang tăng lên.
  - Số lượng đơn vay trong tháng hiện tại (MTD) là 4.3K, có thể tiếp tục tăng vào cuối tháng
- Hồ sơ vay tốt và xấu (Good vs Bad Loans):
  - 86.2% của các khoản vay được xem là Good Loans (khoảng 33.2K đơn), cho thấy tỷ lệ nợ xấu thấp chỉ 13.8% (khoảng 5.3K đơn là Bad Loans).
  - Tổng số tiền nhận từ các khoản vay tốt là $435.8M, trong khi tổng số tiền nhận từ các khoản vay xấu là $37.3M
- Lãi suất trung bình (Average Interest Rate):
  - Lãi suất trung bình là 12.05%, tăng nhẹ 3.5% so với tháng trước
  - Điều này có thể do chính sách ngân hàng hoặc tình hình thị trường tài chính thay đổi, nhưng vẫn trong mức chấp nhận được cho các khoản vay cá nhân hoặc doanh nghiệp nhỏ
- DTI trung bình (Average DTI - Debt-to-Income Ratio):
  - Tỷ lệ DTI trung bình là 13.33%, cho thấy hầu hết người vay có mức nợ không quá cao so với thu nhập, dấu hiệu cho thấy rủi ro về nợ xấu vẫn được kiểm soát
- Phân tích theo mục đích vay (Loan Applications by Purpose):
  - Mục đích vay phổ biến nhất là Debt consolidation với 18K đơn vay, cho thấy nhiều người vay đang tìm cách quản lý nợ hiện tại
  - Các mục đích khác như Credit card (5K), Home improvement (3K), và Small business (2K) cũng đáng chú ý
- Thời hạn khoản vay (Loan Applications by Term):
  - Phần lớn các khoản vay có kỳ hạn 60 tháng (73.2%) so với 36 tháng (26.8%), cho thấy người vay có xu hướng lựa chọn thời hạn dài hơn, có thể để giảm áp lực thanh toán tiền lãi hàng tháng
2. Overview Page
![detail](https://github.com/user-attachments/assets/ba2aaef6-3f9f-4440-89bb-c58ed3a2c1bf) <br />
- Tăng trưởng hồ sơ vay theo tháng (Loan Applications by Month):
  - Số lượng đơn vay tăng dần qua các tháng trong năm. Từ tháng 1 với 2.3K đơn, đến tháng 12 là 4.3K, cho thấy nhu cầu vay vốn tăng đều đặn
- Hồ sơ vay vốn theo thời gian làm việc(Loan Applications by Employee Length):
  - Nhóm có thời gian làm việc 10+ năm chiếm 8.9K đơn vay, nhiều nhất trong tất cả các nhóm, cho thấy những người có công việc ổn định thường có xu hướng vay nhiều hơn.
  - Nhóm có thời gian làm việc dưới 1 năm chiếm 4.6K đơn vay, cho thấy ngay cả những người mới đi làm cũng có nhu cầu vay vốn, có thể để thanh toán nợ hoặc chi phí sinh hoạt.
- Phân tích theo hình thức sở hữu nhà (Home Ownership):
  - Người thuê nhà chiếm phần lớn đơn vay (18.4K so với 17.2K của người thế chấp nhà). Điều này có thể chỉ ra rằng những người thuê nhà có xu hướng cần vay để quản lý các chi phí sinh hoạt hoặc nợ, trong khi người sở hữu nhà có thể vay để trả nợ hoặc vay để mua nhà
3. Detail Page
![overview](https://github.com/user-attachments/assets/4d78ddca-b7af-4faa-88ce-2a3cefef745f) <br />
