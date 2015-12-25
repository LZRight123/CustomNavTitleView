//
//  ViewController.m
//  CustomNavTitleView
//
//  Created by 梁泽 on 15/11/24.
//  Copyright © 2015年 right. All rights reserved.
//

#import "ViewController.h"
#import "NavTitleView.h"
@interface ViewController ()

@end

@implementation ViewController

- (void)viewDidLoad {
    [super viewDidLoad];
    self.navigationController.navigationBar.backgroundColor = [UIColor redColor];
    self.view.backgroundColor = [UIColor blueColor];
    
    [[NSNotificationCenter defaultCenter] addObserver:self selector:@selector(click:) name:UIKeyboardWillShowNotification object:nil];
    NavTitleView *titleView = [NavTitleView create];
    self.navigationItem.titleView = titleView;
    // Do any additional setup after loading the view, typically from a nib.
}

- (void)didReceiveMemoryWarning {
    [super didReceiveMemoryWarning];
    // Dispose of any resources that can be recreated.
}
- (void) click:(NSNotification*)notfication{
//    [NavTitleView showBlurEffectOnView:self.view];
}
- (void) navTitleViewDidClickLeftBtn:(NavTitleView*)view{
    NSLog(@"navTitleViewDidClickLeftBtn");
}

- (void) navTitleViewDidClickRightBtn:(NavTitleView*)view{
    NSLog(@"navTitleViewDidClickRightBtn");
}

- (void) navTitleView:(NavTitleView*)view searchText:(NSString*)text{
    NSLog(@"%@",text);
}
@end
