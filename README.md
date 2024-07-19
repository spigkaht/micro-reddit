Users

  username:string [unique, 4-12 chars, present]
  email:string [unique, present]
  password:string [6-16 chars, present]
  id:integer
  created_at:datetime
  updated_at:datetime

  has_many posts


Posts

  title:string [unique, present]
  body:text [present]
  author_id:integer [present]
  id:integer
  created_at:datetime
  updated_at:datetime

  belongs_to user


Comments
