import sys

def get_status(is_published):
    if is_published:
        return 'PUBLISHED'
    else:
        return 'DRAFT'

def print_status(posts):
    for post in posts:
        print(post['title'] + ' - ' + get_status(post['is_published']))

posts = [
    {'title': 'Post 1', 'is_published': True},
    {'title': 'Post 2', 'is_published': False}
]

print_status(posts)