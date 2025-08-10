This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
# kpghome_next


# ディレクトリ参考
kpghome_next/
├── app/
│   ├── layout.js
│   ├── page.js
│   └── page.module.scss    # ページ固有のスタイル
├── styles/                  # グローバルなSCSS
│   ├── globals.scss        # メインのグローバルスタイル
│   ├── variables.scss      # 変数定義
│   ├── mixins.scss        # ミックスイン
│   ├── components/        # コンポーネント用SCSS
│   │   ├── budget.scss
│   │   ├── modal.scss
│   │   └── button.scss
│   └── layouts/           # レイアウト用SCSS
│       ├── header.scss
│       └── footer.scss
├── components/
│   ├── budget/
│   │   ├── BudgetTable.js
│   │   └── BudgetTable.module.scss  # コンポーネント固有
│   └── modals/
│       ├── AddExpenseModal.js
│       └── AddExpenseModal.module.scss
└── _original/              # 既存CSS参照用




my-kakeibo-app/
├── app/
│   ├── api/                    # API Routes (バックエンド)
│   │   ├── expenses/
│   │   │   ├── route.js        # GET, POST /api/expenses
│   │   │   └── [id]/
│   │   │       └── route.js    # GET, PUT, DELETE /api/expenses/[id]
│   │   ├── categories/
│   │   │   └── route.js        # GET /api/categories
│   │   └── summary/
│   │       └── route.js        # GET /api/summary (月次集計など)
│   ├── expenses/               # 支出管理ページ
│   │   ├── page.js             # 支出一覧ページ
│   │   ├── add/
│   │   │   └── page.js         # 支出追加ページ
│   │   └── [id]/
│   │       └── page.js         # 支出詳細・編集ページ
│   ├── dashboard/              # ダッシュボード
│   │   └── page.js             # 家計簿サマリー
│   ├── components/             # 共通コンポーネント
│   │   ├── ExpenseForm.js      # 支出入力フォーム
│   │   ├── ExpenseList.js      # 支出一覧
│   │   └── Summary.js          # 月次サマリー
│   ├── layout.js               # 全体レイアウト
│   └── page.js                 # ホームページ
├── lib/
│   ├── data.js                 # データ管理（一時的にメモリ保存）
│   └── utils.js                # ユーティリティ関数
├── package.json
└── next.config.js
